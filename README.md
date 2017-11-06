# Tablet Bar Mount

## Zadání

Vaším úkolem je namodelovat držák na tablet na řídítka motocyklu, za účelem použítí tabletu k navigaci.
Držák tabletu je potřeba namontovat na představce řídítek, protože to je nejbezpečnější a zároveň nejpevnějsí misto, které je jezdci snadno na očích.

## Motivace

Nic podobného neexistuje, i přes poptávku motorkářu, čili po splnění úkolu ho můžete OpenSourcovat a publikovat například na Thingiverse nebo podobných webech a býti slavní... :)

### Představce

![představce (http://www.lewisportusa.com/Images/vmar/vmar_barmounts_a.jpg)](barmounts.jpg)
![řídítka (https://spieglerusa.com/media/catalog/product/cache/1/image/736x460/17f82f742ffe127f42dca9de82fb58b1/i/m/img_1937sm_2_4.jpg)](handlebars.jpg)

## Model
Vámi namodelovaný model se bude skládat ze dvou objektů.

  - Horní část modelu s výřezem pro display modelu
  - Spodní část modelu, který se dá přídělat na přestavce řídítek


## Interface modelu

```
module tablet_bar_mount() {}

```

### Horní část

#### Interface

```
module top_part( holder_width,
					holder_height,
					holder_overlay_thickness,
					tablet_width,	
					tablet_height,
					tablet_depth,
					tablet_screen_width,
					tablet_screen_height,
					rounded_corner_radius, 
					connecting_screw_diameter,
					cable_cutout_height,
					cable_cutout_depth) {}
```

#### Argumenty
  - `holder_width, holder_height` jsou rozměry držáku, tloušťka horní části se odvíjí od `tablet_depth` a `holder_overlay_thickness`
  - `holder_overlay_thickness` je tlouštka modelu mezi displayem a horní částí držáku, čili ta část, která překrývá okraje tabletu, kde není display
  - `tablet_width, tablet_height, tablet_depth` jsou rozměry tabletu
  - `tablet_screen_width, tablet_screen_height` jsou rozměry displaye tabletu, čili otvor, ktery bude vyříznut do horní části držáku.
  - `rounded_corner_radius` poloměr zakřivení rohů, pokud je argument nulový tak rohy nejsou zaoblené
  - `connecting_screw_diameter` průměr šroubu, které jsou drží horní a spodní část držáku
  - `cable_cutout_height` výška vyřezu pro kabely
  - `cable_cutout_depth` tloušťka výřezu pro kabely

![top_part](top_part_no_rouded_corners.png)
![top_part_bottom_view](top_part_no_rouded_corners_bottom_view.png)
![top_view_side_view](top_part_side_view.png)
![top_rouded](top_rouded.png)

### Spodní část

#### Interface

```
module bottom_part( holder_width,
						holder_height,
						holder_thickness,
						nut_diameter,
						nut_depth,
						screw_diameter,
						screw_head_diameter,
						screw_head_depth,
						raiser_width,
						raiser_height,
						raiser_depth,
						raiser_inlet_wall_thickness,
						raiser_inlet_top_thickness,
						bar_diameter,
						bar_location,
						raisers_spacing
						) {}
```



#### Argumenty

  - `holder_width, holder_height` jsou rozměry držáku
  - `holder_thickness` je tloušťka spodní části držáku ne kterém bude ležet tablet
  - `nut_diameter` průměr šestihranné matky
  - `nut_depth` tloušťka matky, která bude zasazena do spodní části držáku
  - `screw_diameter` průměř šroubu, který se pasuje do představce řídítek
  - `screw_head_diameter` průměr hlavičky šroubu, který pasuje do představce řídítek
  - `screw_head_depth` výška hlavičky šroubu, který bude zapuštěn do spodní části modelu
  - `raiser_width` je šířka reálného představce řídítek
  - `raiser_height` je délka realného představce řídítek 
  - `raiser_depth` je výška reálného představce řídítek
  - `raiser_inlet_wall_thickness` je tloušťka objímky představce řídítek
  - `raiser_inlet_top_thickness` je tloušťka horní části objímky představce
  - `bar_diameter` průměr řídítek
  - `bar_location` je délka změřena od spodní části představce k vrchní bodu řídítek
  - `raisers_spacing` je rozteč středu šroubu představců, nezáleží zda horních či spodních, vzdálenosti horních a spodních šroubů jsou vždy stejné



#### Objímka představce řídítek

![riser_holder](riser1.png)
![riser_holder](riser2.png)
![riser_holder](riser3.png)

#### Kombinace objímek řídítek
![riser_holder](2risers_top_view.png)

#### Spodní část držáku tabletu
  - Díry ve spodním držáku tabletu, nejsou skrz a slouží k vložení matiček, čili jsou pětihranné
 

![tablet_bottom](tablet_bottom_2.png)
![tablet_bottom](tablet_bottom.png)

#### Kombinace horního a spodního držáku tabletu
![tablet_holder](tablet_holder.png)

#### Kombinace objímky a spodního držáku tabletu
![riser_bottom](riser_bottom.png)
![riser_bottom](riser_bottom2.png)
![riser_bottom_side_view](riser_bottom_side_view.png)

#### Celý držák

![](holder_complete.png)
![](holder_complete2.png)

#### Možnost nastevení pozorovacího úhlu
![](holder_complete_rotated.png)
![](holder_complete_rotated2.png)


