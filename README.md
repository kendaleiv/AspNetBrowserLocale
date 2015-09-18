# AspNetBrowserLocale

Provides functionality for showing DateTime information respecting the time zone of the users browser using Razor.

## Usage (Razor)

In **_Layout.cshtml** or a similar file, add the following:

```
@using RimDev.AspNetBrowserLocale

@Html.InitializeLocaleDateTime()
```

Then, for each DateTime (or, nullable DateTime) value you wish to display:

```
@using RimDev.AspNetBrowserLocale
@{
    var myDateTime = new DateTime(2015, 1, 1);
}

@Html.BrowserDisplay(myDateTime)
```

## License

MIT
