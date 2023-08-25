# Minecraft_Bear_code
Minecraft bear

![Екранна снимка 2023-08-24 223448](https://github.com/HROMAFOX/Minecraft_Bear_code/assets/113515660/73bbf355-6195-4b1c-8548-de1f1b3f1d79)

Халба с бира

![Екранна снимка 2023-08-24 230848](https://github.com/HROMAFOX/Minecraft_Bear_code/assets/113515660/4a461e6d-e643-4e4d-80f5-fa7dd5e0c06c)

Празна халба

![Екранна снимка 2023-08-24 230658](https://github.com/HROMAFOX/Minecraft_Bear_code/assets/113515660/16dc63e6-4d71-4e37-b625-ad3229b0b733)

Ефекти от бирата(Всички ефекти са по 15 секунди)

![Екранна снимка 2023-08-24 230134](https://github.com/HROMAFOX/Minecraft_Bear_code/assets/113515660/a5c76dfa-06c5-4dcd-bd65-43022545bb69)

Така се поставят командните блокове




<pre class="wp-block-code">
<code>🍻Команден блок 1(Repeat/Unconditional/Always Active) 
/execute as @e[type=player, nbt={Inventory:[{Slot:-106b, id:"minecraft:player_head", tag:{display:{Name:"{\"text\":\"Mug with Beer\",\"color\":\"white\"}", Lore:['{"color":"yellow","text":"с 15% алкохол"}','{"color":"green","text":"Пие се с F"}']}}}]}] at @s run playsound minecraft:entity.generic.drink player @s ~ ~ ~ 0.65 1 0

🍻Команден блок 2(Chain/Conditional/Always Active) 
/execute as @e[type=player, nbt={Inventory:[{Slot:-106b, id:"minecraft:player_head", tag:{display:{Name:"{\"text\":\"Mug with Beer\",\"color\":\"white\"}", Lore:['{"color":"yellow","text":"с 15% алкохол"}','{"color":"green","text":"Пие се с F"}']}}}]}] at @s run scoreboard players add @s BeerDrinking 1

🍻Команден блок 3(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] at @s run clear @s minecraft:player_head{display:{Name:"{\"text\":\"Mug with Beer\",\"color\":\"white\"}", Lore:['{"color":"yellow","text":"с 15% алкохол"}','{"color":"green","text":"Пие се с F"}']}} 1

🍻Команден блок 4(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] at @s run give @s minecraft:player_head{display:{Name:"{\"text\":\"Empty Mug\",\"color\":\"white\"}", Lore:['{"color":"green","text":"напълни ме"}']},SkullOwner:{Id:[I;1176276444,967657176,-1996008735,-1173811510],Properties:{textures:[{Value:"eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvM2Y1NmEyNmE5NDljMTMzYWI5NTAyMTFkZGRhZmViMjU1MWMwNTJlMWNmZmY2MTcyZmM2OGNkYTMyMTliMDg0In19fQ=="}]}}} 1

🍻Команден блок 5(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] at @s run playsound minecraft:entity.player.burp player @s ~ ~ ~ 10 1 1

🍻Команден блок 6(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] as @s run effect give @s minecraft:nausea 15 0 true

🍻Команден блок 7(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] as @s run effect give @s minecraft:darkness 15 0 true

🍻Команден блок 8(Chain/Conditional/Always Active) 
/execute as @e[type=player, scores={BeerDrinking=5..}] at @s run scoreboard players set @s BeerDrinking 0

🍻Тази команда трябва да бъди написана в чата веднъж! 
/scoreboard objectives add BeerDrinking dummy

🍻Обикновен Команден блок с бутон за взимане на бирата! 
/summon minecraft:item ~ ~1 ~ {Item:{id:"minecraft:player_head",Count:1b,tag:{display:{Name:"{\"text\":\"Mug with Beer\",\"color\":\"white\"}", Lore:['{"color":"yellow","text":"с 15% алкохол"}','{"color":"green","text":"Пие се с F"}']},SkullOwner:{Id:[I;-1513351130,1351370996,-1551837317,-2013369534],Properties:{textures:[{Value:"eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvNDA1M2UyNjg2N2JiNTc1MzhlOTc4OTEzN2RiYmI1Mzc3NGUxOGVkYTZmZWY1MWNiMmVkZjQyNmIzNzI2NCJ9fX0="}]}}}}}
</code></pre>
