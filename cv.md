# Sergei Pustovoi
![myPhoto](/img/im.jpg)
## Contacts
   * **Tel:** _+7 961-951-961-8_ 
   * **Telegram** [_Epimetey1_](https://t.me/epimetey1/)
   * **E-mail:** _epimetey@yandex.ru_
   * **Discord nick in RSSchool** [_@Epimetey_](https://discordapp.com/users/919839678352465982/)
 
## About me
   - **Age:** _44_
   - **Sex:** _male_
   - **Profession:** _Security_
   - **My goal:** _I want to master modern programming. My goal is to implement my project.. To do this, I need knowledge of full stack and back-end programming._
## Skills 
   - **Python**
      - _Rank: 6 kyu / Total Completed Kata: 37_
   - **HTML, CSS & Git** 
      - _Poor_

## Code examples
   - Python
   ```
   def peak_height(mountain):

    ### Проверка длины строк. При не соответствии длины - дополняем в конце нужное число “ ”. предварительно доводим до четного числа длину строки.
    len_ver = len(mountain)
    len_hor = len(mountain[0])
    for i in range(0,len_ver):
        if len_hor < len(mountain[i]):
            len_hor = len(mountain[i])
    if len_hor // 2 < len_hor / 2:
        len_hor += 1
    for i in range(0,len_ver):
        mountain[i] = mountain[i].ljust(len_hor," ")
 
    ### Создаем массив и переводим в него оцифрованные данные:"  "  = 0, "^" = 1
    mass = []
    mass2 = []
    for i in range(len_ver):
        mass.append([0]*len_hor)
    for i in range(len_ver):
        mass2.append([0]*len_hor)

    for v in range(0,len_ver):
        for h in range(0,len_hor):
            mass [v][h] = 1 if mountain[v][h] == '^' else 0
    height = 0                          # высота (по умолчанию 0)
    
    ### Проверяем наличие 1 в массиве. 
    ### Если sum < 5 – выдаем результат подсчета высоты - 1,  если summ = 0 выдаем - 0 
    ###(закоменчено. хз почему глючит проверка. ну и пофигу. без нее работает)
    def check(mass):
        summ = 0            
        for i in range (0,len_ver):
            for x in mass[i]: 
                summ += x
        return summ                     #----------------------------
    summ = check(mass)  
    if summ == 0:
        return height                 ################ return height
#    elif summ < 1:
#        return 1                     ################ return 1
    else:
        height +=1

    #len_ver_var = len_ver
    # Первые и последние ячейки исключаем из проверки
    for n in range(max(len_ver,len_hor)):
        for i in range (1,len_ver-1):
            for j in range (1,len_hor-1):
                if mass [i-1][j] == 0 or mass [i][j-1] == 0 or mass [i+1][j] == 0 or mass [i][j+1] == 0:
                    mass2 [i][j] = 0
                else:
                    mass2 [i][j] = 1
        # Обнуляем нижнюю и верхниюю строки, первые и последние ячейки (единожды)
        if n == 0:
            for i in range (0,len_ver):
                mass [i][0] = 0
                mass [i][-1] = 0
            for j in range (0,len_hor):
                mass [0][j] = 0
                mass [-1][j] = 0

        # Проверяем остаточную сумму
        summ = check(mass2)  
        if summ < 1:
            return height                  ################ return height
        else:
            height +=1
    
        # Переносим данные из mass2 в mass за одно обнуляя массив mass2
        for v in range (0,len_ver):
            for h in range (0,len_hor):    
                mass [v][h] = mass2 [v][h]
                mass2 [v][h] = 0
        n += 1
    return height                                   ################ РЕЗУЛЬТАТ
   ```
   - JS
   ```
   none
   ```

## Work experience
   - Associate professor of the university (19 years)
   - Content manager & Author of technical articles (2.5 year)

## Education 
   - Programming  
      - Python _(average)_       
         + _literature, guides, YouTube video, etc._
         + _not completed Stepik courses_
      - JavaScript _(none)_      
         + _RS School_
      - Delphy _(average)_      
         + _Independent learning. Several PC applications were written (20 years ago)_         
   - Other 
      - Electrical engineer
      - Cand. Sc. (Agriculture)
      - Pedogog of higher education
      - Copywriter

## Language 
    - English - A2
    - Russian - native
