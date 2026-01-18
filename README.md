# QGIS Layouts 2025
Francis J Adair<br>
fadair206@icloud.com<br>
[Personal Website](https://fadair206.wordpress.com)

QGIS template layouts for professional figure production.<br>
Available for download on [QGIS Layout-Hub](https://qgis-hub.fast-page.org/layouts.php).

### Landscape

<img src="QGIS Project A3 Landscape.png" alt="QGIS Project A3 Landscape"/>

### Portrait

<img src="QGIS Project A3 Portrait.png" alt="QGIS Project A3 Portrait"/>

## Summary Tables

| Layout Item         | Description                                                                                     |
|---------------------|-------------------------------------------------------------------------------------------------|
| Project Title       | [%@project_title%] is set in the project properties.                                             |
| Figure Title        | [%@Figure_Title%] is set in the layout variables.                                               |
| Legend              | Small font size and spacing allows for more legend space.                                        |
| Meta                | [%@layout_name%]<br>[% title(format_date( now(), 'dd MMMM yyyy'))%]<br>[%@Figure_Author%]<br>[%@layout_pagewidth%] x [%@layout_pageheight%]  mm       |
| Notes               | Let your imagination run wild.                                                                  |
| Inset Map           | Make all but your basemap invisible then check the ‘Lock layers’ box.<br>Uses a red outline Overview of the Main Map. |
| Scale Bar           | Set to ‘Fixed width’ using units and segments to fit different scales.                          |
| Scale Number        | Numeric scale underneath the scale bar.                                                         |
| CRS Description     | [%@project_crs_description%]<br>[%@project_crs%]                                                 |
| Corner Coordinates  | NE Corner<br>[%round(x_max(map_get(item_variables('Main Map'), 'map_extent')))%],<br>[%round(y_max(map_get(item_variables('Main Map'), 'map_extent')))%]<br>SW Corner<br>[%round(x_min(map_get(item_variables('Main Map'), 'map_extent')))%],<br>[%round(y_min(map_get(item_variables('Main Map'), 'map_extent')))%] |
| QGIS Version        | Made with QGIS [% @qgis_short_version %] on [%title( @qgis_os_name )%]                          |
| Attribution         | F J Adair; [%array_to_string(map_credits('Main Map'))%]                           |
| Sidebar Frame       | Width of 60 mm and contains everything except the Main Map and North Arrow.                     |
| North Arrow         | Top right corner.                                                                                |
| Main Map            | Select between grid elements ‘Coordinates’, ‘Interior Ticks’, ‘Solid Grid’.                    |

### Guides

| #  | **Landscape**                     |                                  | **Portrait**                      |                                  |
|----:|----------------------------------:|---------------------------------:|----------------------------------:|---------------------------------:|
|    | Horizontal Guides (mm)           | Vertical Guides (mm)            | Horizontal Guides (mm)           | Vertical Guides (mm)             |
|  1 | 6.00                             | 6.00                             | 6.00                             | 6.00                             |
|  2 | 7.85                             | 6.30                             | 7.85                             | 6.30                             |
|  3 | 8.15                             | 8.15                             | 8.15                             | 8.15                             |
|  4 | 13.85                            | 25.85                            | 13.85                            | 25.85                            |
|  5 | 14.15                            | 26.15                            | 14.15                            | 26.15                            |
|  6 | 19.85                            | 35.85                            | 19.85                            | 35.85                            |
|  7 | 20.15                            | 36.00                            | 20.15                            | 36.00                            |
|  8 | 25.85                            | 36.15                            | 25.85                            | 36.15                            |
|  9 | 26.15                            | 45.85                            | 26.15                            | 45.85                            |
| 10 | 218.85                           | 46.15                            | 341.85                           | 46.15                            |
| 11 | 219.15                           | 63.85                            | 342.15                           | 63.85                            |
| 12 | 224.85                           | 65.70                            | 347.85                           | 65.70                            |
| 13 | 225.15                           | 66.00                            | 348.15                           | 66.00                            |
| 14 | 264.85                           | 396.85                           | 387.85                           | 273.85                           |
| 15 | 265.15                           | 397.15                           | 388.15                           | 274.15                           |
| 16 | 270.85                           | 405.85                           | 393.85                           | 282.85                           |
| 17 | 271.15                           | 406.15                           | 394.15                           | 283.15                           |
| 18 | 276.85                           | 411.85                           | 399.85                           | 288.85                           |
| 19 | 277.15                           | 412.15                           | 400.15                           | 289.15                           |
| 20 | 282.85                           | 414.00                           | 405.85                           | 291.00                           |
| 21 | 283.15                           |                                  | 406.15                           |                                  |
| 22 | 288.85                           |                                  | 411.85                           |                                  |
| 23 | 289.15                           |                                  | 412.15                           |                                  |
| 24 | 291.00                           |                                  | 414.00                           |                                  |

## FAQ

* The portrait layout allows for more legend items and provides greater vertical space.
* All items have either a black or transparent frame activated with 0.3 line thickness.
* Verdana is used for its readability at small font sizes and compatability with software updates.

## License

CC0 1.0 Universal (CC0 1.0) Public Domain Dedication