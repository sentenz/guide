# App Resources

[App Resources](https://developer.android.com/guide/topics/resources/providing-resources) are additional files and static content used in the code, such as bitmaps, layout definitions, user interface strings and values, animation instructions, and more.

- [Resource Types](#resource-types)
- [Syntax](#syntax)
  - [Syntax for C](#syntax-for-c)
  - [Syntax for Go](#syntax-for-go)
  - [Syntax for XML](#syntax-for-xml)
- [See also](#see-also)

Always externalize app resources such as images and strings from the code, so that you can maintain them independently. Also provide alternative resources for specific device configurations, by grouping them in specially-named resource directories.

## Resource Types

Place [resource types](https://developer.android.com/guide/topics/resources/available-resources) in a specific subdirectory of the project's `resource/` directory.

Resource directories supported inside project `resource/` directory.

| Directory | Resource Type                                                     |
| --------- | ----------------------------------------------------------------- |
| animator/ | Files that define property animations.                            |
| color/    | Files that define a state list of colors.                         |
| drawable/ | Bitmap files (.png, .jpg, .gif).                                  |
| mipmap/   | Drawable files for different launcher icon densities.             |
| layout/   | Files that define a user interface layout.                        |
| menu/     | Files that define app menus.                                      |
| raw/      | Arbitrary files to save in their raw form.                        |
| values/   | Files that contain values, such as strings, integers, and colors. |
| xml/      | Arbitrary XML files that can be read at runtime.                  |
| font/     | Font files.                                                       |

## Syntax

The syntax to reference a resource in code:

```bash
[<package_name>.]<resource_type>.<resource_name>
```

- `package_name`
  > The name of the package in which the resource is located.

- `resource_type`
  > The subclass for the resource type.

- `resource_name`
  >  Either the resource filename without the extension or the name attribute value.

### Syntax for C

```bash
[<package_name>_]<resource_type>_<resource_name>
```

### Syntax for Go

```bash
[<package_name>.]<resource_type>_<resource_name>
```

### Syntax for XML

```bash
@[<package_name>:]<resource_type>/<resource_name>
```

## See also

- Android [app resources](https://developer.android.com/guide/topics/resources/providing-resources) article.
- Android [resource types](https://developer.android.com/guide/topics/resources/available-resources) article.
- Microsoft [app resources](https://docs.microsoft.com/en-us/windows/uwp/app-resources/) article.
