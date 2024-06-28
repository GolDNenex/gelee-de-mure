
# gelee-de-mure

`Gelée de mûre` is a dark/purple theme for Jellyfin.

## Installation:

### With Jellyfin (Recommended):
Everyone will be able to use this theme. Users can opt out in they're settings (display > `Disable server-provided custom CSS code`)

Copy the following code, in jellyfin > settings > general > `Custom css code`

```
@import url("
https://raw.githubusercontent.com/GolDNenex/gelee-de-mure/main/theme.css");
```

If you want to stay fully self-hosted, you will need to host yourself the css (with nginx for example), its highly recommanded, even more if you want to customise assets (see [Customization](#quick-start)).

### With [Stylus](https://github.com/openstyles/stylus) (Limited):

 Only you will be able to see the theme. Ideal if the owner of the jellyfin server don't want to install this theme or already use another.

## Customization :

After installing, multiple part of the theme can be edited. Modification need to be placed under the `@import` we made before.

You can modify multiple variable in the same `:root { ... }`

| Designation  | Variable name | Default |
| ------------- | ------------- | ------------- |
| Accent color | --accent-color  | #916de4  |
| Accent color darker  | --accent-color-darker  | #53417b  |
| Corner radius | --corner-radius | 12px |
| Logo | --logo-img | embedded* |
| Logo banner | --banner-img | embedded* |
| Login background image | --login-bg-img | embedded* |

(* is included as base64 inside the css)

### Accent color:

```
:root {
    --accent-color: #916de4;
}
```

### Accent color darker:

```
:root {
    --accent-color-darker: #53417b;
}
```

### Corner radius:

```
:root {
    --corner-radius: 12px;
}
```

### Logo:

```
:root {
    --logo-img: url("https://your_domain_name.nice/logo.png") !important;
}
```

### Logo banner:

```
:root {
    --logo-img: url("https://your_domain_name.nice/logo-banner.png") !important;
}
```

### Logo banner:
Jellyfin generate a `splashscreen.png` file in the `data` folder that can be use for this.

```
:root {
    --logo-img: url("https://your_domain_name.nice/splashscreen.png") !important;
}
```

## Compatibility: 
Compatible with `Jellyfin >= 10.9.0`.

If you are running a older version, use the previous [version](https://github.com/GolDNenex/gelee-de-mure/tree/94b5d218435e1f4c57ff63ca47cfda9a93909801) BUT note that this version is concidered `archived`.