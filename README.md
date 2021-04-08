# Elixir Course and Testing Examples

# Notes

## Maps
### Update Maps
  
> Example 1
```elixir
iex> colors = %{primary: "blue"}
%{primary: "blue"}

iex> Map.put(colors, :primary, "red")
%{primary: "red"}

iex> colors
%{primary: "blue"}

```

> Example 2
```elixir
iex> colors = %{primary: "blue"}
%{primary: "blue"}

iex> %{colors | primary: "red"}
%{primary: "red"}

iex> colors
%{primary: "blue"}

```

### Add Map
> Example 1
```elixir
iex> colors = %{primary: "blue"}
%{primary: "blue"}

iex> Map.put(colors, :secondary, "red")
%{primary: "blue", secondary: "red"}

iex> colors
%{primary: "blue", secondary: "red"}

```

### Keyword List
```elixir
iex> colors = [{:primary, "red"}, {:secondary, "green"}]
[primary: "red", secondary: "green"]
iex> colors[:primary]
"red"
```