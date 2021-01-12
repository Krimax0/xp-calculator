f = open('text.txt', 'w')

language = int(input("Eng-1, Rus-2:"))

if language == 2:
	exp = int(input("Начальное кол-во XP:"))
	Levels = int(input("Кол-во уровней:"))
	dsa = int(input("Режим(0-С показателем уровня, 1-Без показателя):"))
	textlevel = " - уровень:"
else:
	exp = int(input("Initial quantity XP:"))
	Levels = int(input("Number of levels:"))
	dsa = int(input("Mode(1-Assistant mode, 2-None):"))
	textlevel = " - level:" 

exp1 = exp
polovinaexp = exp / 10	
i = 1
level = 1
while i <= int(Levels):
	if dsa == 1:
		a = (str(exp) + textlevel + str(level) + "\n")
		f.write(a)
		print(a)
		level += 1
		exp = (exp1 + polovinaexp) * level
		exp = round(exp)
		i += 1
		polovinaexp = exp / 10
	elif dsa == 2:
		a = (str(exp) + "\n")
		f.write(a)
		print(a)
		level += 1
		exp = (exp1 + polovinaexp) * level
		exp = round(exp)
		i += 1
		polovinaexp = exp / 10
	else:
		a = (str(exp) + textlevel + str(level) + "\n")
		f.write(a)
		print(a)
		level += 1
		exp = (exp1 + polovinaexp) * level
		exp = round(exp)
		i += 1
		polovinaexp = exp / 10


if language == 2:
	print("Просмотрите файл text.txt созданный в данной директории")
else:
	print("View the text.txt file created in this directory")
