# Tablet Bar Mount

## Zadání

Vaším úkolem je namodelovat držák na tablet na řídítka motocyklu, za účelem použítí tabletu k navigaci.
Držák tabletu je potřeba namontovat na představce řídítek, protože to je nejbezpečnější a zároveň nejpevnějsí misto, které je jezdci snadno na očích.

### Představce

![představce (http://www.lewisportusa.com/Images/vmar/vmar_barmounts_a.jpg)](barmounts.jpg)
![řídítka (https://spieglerusa.com/media/catalog/product/cache/1/image/736x460/17f82f742ffe127f42dca9de82fb58b1/i/m/img_1937sm_2_4.jpg)](handlebars.jpg)

## Interface modelu

```
module tabletBarMount() {}

module top_part( tablet_width,
				    tablet_height,
				    tablet_thickness,
				    rounded_corner, 
				    overlay,
				    screw_diameter,
				    cable_cutout_height,
				    cable_cutout_thickness) {}

module bottom_part() {}

```

### Top Part

Top part, bez zaoblenych rohu

```
top_part( 
			tablet_width = ,
			tablet_height = ,
			tablet_thickness = ,
			rounded_corner = , 
			overlay = ,
			screw_diameter = ,
			cable_cutout_height = ,
			cable_cutout_thickness = 
		 )
				    
```
![top_part](top_part_no_rouded_corners.png)
![top_part_bottom_view](top_part_no_rouded_corners_bottom_view.png)
![top_view_side_view](top_part_side_view.png)


Top part, se zaoblenymi rohy // TODO

### Bottom part

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


