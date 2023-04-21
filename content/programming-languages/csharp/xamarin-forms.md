---
date: 2017-11-08T18:34:45-05:00
title: "Xamarin Forms"
seo_title: "Xamarin Forms Mobile Development | C# | 🦒"
subheader:
     greeting: C# - Programming Language
     description: This course will cover everything you need to know to get started with Xamarin Forms mobile development
description: This course will cover everything you need to know to get started with Xamarin Forms mobile development
author: 🦒
image: building-a-mad-libs-game.png
video: 
url: /programming-languages/csharp/xamarin-forms-tutorial/
weight: 33
---

## XAML Intro

```html
<Button Text="Click Me" Clicked="HandleButtonClick"/>
```

```cs
public void HandleButtonClick(object sender, EventArgs args)
{
    Console.WriteLine("You Clicked Me!");
}
```

## Building a text entry

```html
<StackLayout>
    <Entry
        x:Name="TodoInput"
        Text=""
        TextChanged="HandleTextChanged"
        Completed="HandleTextCompleted"
    />
    
    <StackLayout x:Name="TodoList">

    </StackLayout>
</StackLayout>
```

```cs
public void HandleTextChanged(object sender, TextChangedEventArgs args)
{
    Console.WriteLine(args.NewTextValue);
}

public void HandleTextCompleted(object sender, EventArgs args)
{
    Label newTodo = new Label();
    newTodo.Text = TodoInput.Text;
    TodoList.Children.Add(newTodo);
    TodoInput.Text = "";
}
```

## MVVM Intro

- Model is what defines what the actual data we're working with looks like
- View is the XAML
- ViewModel connect these two things together

## Building the TodoItem Model

```cs
using System;
namespace AppPractice
{
    public class TodoItem
    {
        public string TodoText { get; set; }
        public bool Complete { get; set; }

        public TodoItem(string TodoText, bool Complete)
        {
            this.Text = TodoText;
            this.Complete = Complete;
        }
    }
}
```

## Building the TodoListViewModel

```cs
using System;
using System.Collections.ObjectModel;

namespace AppPractice
{
    public class TodoListViewModel
    {

        public ObservableCollection<TodoItem> TodoItems { get; set; };

        public TodoListViewModel()
        {
            TodoItems = new ObservableCollection<TodoItem>();

            TodoItems.Add(new TodoItem("First Todo", true));
        }
    }
}
```

## Wiring the ViewModel to the View

- Don't forget to remove all the old handlers and code

```html
<ListView x:Name="TodoList" ItemsSource="{Binding TodoItems}">
    <ListView.ItemTemplate>
        <DataTemplate>
            <ViewCell>
                <Label Text="{Binding Text}"/>
            </ViewCell>
        </DataTemplate>
    </ListView.ItemTemplate>
</ListView>
```

## Adding a new todo

```cs
using System.Windows.Input;
using Xamarin.Forms;
...

public ICommand AddTodoCommand => new Command(AddTodoItem);
public string NewTodoInputValue { get; set; }
void AddTodoItem()
{
    TodoItems.Add(new TodoItem(NewTodoInputValue, false));
}
```

```html
<Entry
    x:Name="TodoInput"
    Text="{Binding NewTodoInputValue}"
    ReturnCommand="{Binding AddTodoCommand}"
/>
```

## Adding a trash icon

- Download the [trash icon](/assets/delete.png)

```cs
<FlexLayout JustifyContent="SpaceBetween" AlignItems="Center" Padding="20, 0">
    <Label Text="{Binding TodoText}"/>
    <ImageButton
        Source="delete.png"
        Scale="0.5"
        BackgroundColor="Transparent"   
    />
</FlexLayout>
```

## Removing a todo

```cs
public ICommand RemoveTodoCommand => new Command(RemoveTodoItem);
void RemoveTodoItem(object o)
{
    TodoItem todoItemBeingRemoved = o as TodoItem;
    TodoItems.Remove(todoItemBeingRemoved);
}
```

```html
<ImageButton
    Command="{Binding Path=BindingContext.RemoveTodoCommand, Source={x:Reference TodoList}}"
    CommandParameter="{Binding .}"
    Source="delete.png"
    Scale="0.5"
    BackgroundColor="Transparent"   
/>
```

## Adding a checkbox

- Manage NuGet Packages -> "Input Kit"

```html
xmlns:input="clr-namespace:Plugin.InputKit.Shared.Controls;assembly=Plugin.InputKit"
...

<ContentView>
    <FlexLayout AlignItems="Center">
        <input:CheckBox
            IsChecked="{Binding Complete}"
        />
        <Label Text="{Binding TodoText}" Margin="20, 0"/>
    </FlexLayout>
</ContentView>
```

## Wiring up the toggle button

```html
<input:CheckBox
    IsChecked="{Binding Complete}"
/>
```
