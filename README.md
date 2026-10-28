# goit-js-hw-04
Задача 1. Пакування товарів

Виконуй це завдання у файлі task-1.js


Оголоси функцію isEnoughCapacity, яка очікує два параметри:

products — об’єкт, у якому ключі містять назви товарів, а значення — кількість цих товарів. Наприклад, { apples: 2, grapes: 4 }.
containerSize — число, максимальна кількість одиниць товарів, яку в себе може вмістити контейнер.


Функція обчислює загальну кількість товарів в об'єкті products і повертає true, якщо вона менша або дорівнює containerSize, і false — якщо ні.



Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

console.log(
  isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
  isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
  isEnoughCapacity({ apples: 1, lime: 5, tomatos: 3 }, 14)
); // true

console.log(
  isEnoughCapacity({ apples: 18, potatos: 5, oranges: 2 }, 7)
); // false



Залиш цей код для перевірки ментором.



Вимоги

Оголошено функцію isEnoughCapacity(products, containerSize).
Виклик isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8) повертає true.
Виклик isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12) повертає false.
Виклик isEnoughCapacity({ apples: 1, lime: 5, tomatos: 3 }, 14) повертає true.
Виклик isEnoughCapacity({ apples: 18, potatos: 5, oranges: 2 }, 7) повертає false.
Виклик з будь-якими валідними аргументами повертає правильне значення.
Результати всіх викликів виведено в консоль.


Задача 2. Розрахунок калорій

Виконуй це завдання у файлі task-2.js


Оголоси функцію calcAverageCalories, яка очікує один параметр days — масив об'єктів. Кожен об'єкт описує день тижня та кількість калорій calories, спожитих спортсменом у цей день. Функція повертає середньодобове значення калорій за тиждень.



Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.



console.log(
  calcAverageCalories([
    { day: "monday", calories: 3010 },
    { day: "tuesday", calories: 3200 },
    { day: "wednesday", calories: 3120 },
    { day: "thursday", calories: 2900 },
    { day: "friday", calories: 3450 },
    { day: "saturday", calories: 3280 },
    { day: "sunday", calories: 3300 }
  ])
); // 3180

console.log(
  calcAverageCalories([
    { day: "monday", calories: 2040 },
    { day: "tuesday", calories: 2270 },
    { day: "wednesday", calories: 2420 },
    { day: "thursday", calories: 1900 },
    { day: "friday", calories: 2370 },
    { day: "saturday", calories: 2280 },
    { day: "sunday", calories: 2610 }
  ])
); // 2270

console.log(
  calcAverageCalories([])
); // 0



Залиш цей код для перевірки ментором.



Вимоги

Оголошено функцію calcAverageCalories(days).
Перший виклик (масив із семи днів) повертає 3180.
Другий виклик (масив із семи днів) повертає 2270.
Виклик з порожнім масивом [] повертає 0.
Виклик з будь-яким валідним масивом повертає правильне середнє значення.
Результати всіх викликів виведено в консоль.


Задача 3. Профіль гравця

Виконуй це завдання у файлі task-3.js


Об’єкт profile описує профіль користувача на ігровій платформі. У його властивостях зберігається ім’я профілю username та кількість активних годин playTime, проведених у грі.



const profile = {
  username: "Jacob",
  playTime: 300,
};



Доповни об’єкт profile методами для роботи з його властивостями.

Метод changeUsername(newName) повинен приймати рядок (нове ім’я) в параметр newName та змінювати значення властивості username на нове. Нічого не повертає.
Метод updatePlayTime(hours) повинен приймати число (кількість годин) у параметр hours та збільшити на нього значення властивості playTime. Нічого не повертає.
Метод getInfo() має повертати рядок формату <Username> has <amount> active hours!, де <Username> — це ім’я профілю, а <amount> — кількість ігрових годин.


Встав код нижче після оголошення методів для перевірки. Залиш його для перевірки ментором.



console.log(profile.getInfo()); // "Jacob has 300 active hours!"

profile.changeUsername("Marco");
console.log(profile.getInfo()); // "Marco has 300 active hours!"

profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"



Залиш цей код для перевірки ментором.



Вимоги

Значення змінної profile — це об'єкт з властивостями username, playTime, getInfo, changeUsername і updatePlayTime.
Значення властивостей getInfo, changeUsername і updatePlayTime — функції.
Для звертання до властивостей об'єкта в його методах використано this.
Виклик profile.getInfo() до змін повертає "Jacob has 300 active hours!".
Виклик profile.changeUsername("Marco") змінює username на "Marco", після чого profile.getInfo() повертає "Marco has 300 active hours!".
Виклик profile.updatePlayTime(20) збільшує playTime на 20, після чого profile.getInfo() повертає "Marco has 320 active hours!".
Результати всіх викликів console.log виведено в консоль.
Завдання очікує виконання

Дедлайн
23:45, 8 листоп.


Здай домашнє 