# Задание №1
```
cut -d: -f1 /etc/passwd |sort
```
![image](https://github.com/user-attachments/assets/6d4f74f8-172e-4b3a-ad54-44fed79a4f8b)
***

# Задание №2
```
cat /etc/protocols | awk '{print $2, $1}' | sort -rn | head -n 5 | awk '{printf "%d %s\n", $1, $2}'
```
![image](https://github.com/user-attachments/assets/ca3a0bec-4d97-409c-885c-8a3bafc605ab)
***

## Задание №3
```
#!/bin/bash
text=$1
size=${#text}
echo -n "+"
for ((i = -2; i < size; i++))
do
echo -n "-"
done
echo "+"
echo "| $text |"
echo -n "+"
for ((i = -2; i < size; i++))
do
echo -n "-"
done
echo "+"
```
![image](https://github.com/tel1ce/alexy_pract1/blob/main/image.png)
