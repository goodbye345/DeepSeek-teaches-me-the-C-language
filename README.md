Это первый урок по языку прогромирования С который предложил мне DeepSeek

.........................................................................................................

Прекрасно, что у вас Ubuntu! Это отличная ОС для разработки на C. Адаптирую урок под ваши условия. 🐧

Урок 1 (адаптирован для Ubuntu + Sublime Text)
Цель: Написать первую программу, используя Ubuntu и Sublime Text.

1. Проверка компилятора GCC
В Ubuntu GCC обычно уже установлен. Проверим:

bash
Copy
gcc --version
Если команда выводит версию (например, 9.4.0), можно переходить к коду.
Если нет, установите GCC:

bash
Copy
sudo apt update && sudo apt install gcc -y
2. Настройка Sublime Text
Установите пакет для удобной работы с C (опционально):
Через Ctrl+Shift+P → Install Package Control → затем установите пакеты:

C Improved (лучшая подсветка синтаксиса).

Terminal (для запуска терминала прямо из редактора).

3. Создайте файл hello.c
Откройте Sublime Text → File → New File → сохраните как hello.c.

Вставьте код:

c
Copy
#include <stdio.h>

int main() {
    printf("Hello, Ubuntu!\n");  // Измените приветствие
    return 0;
}
4. Компиляция и запуск через терминал
Откройте терминал в папке с файлом:

Через Sublime Text: Tools → Terminal → Open Terminal Here.

Или через проводник: правой кнопкой в папке → Open in Terminal.

Скомпилируйте и запустите:

bash
Copy
gcc hello.c -o hello  # Компиляция
./hello               # Запуск
Результат:

Copy
Hello, Ubuntu!
Задание:
Модифицируйте программу, чтобы она выводила ваш имя и любимый цвет. Например:

c
Copy
printf("Привет! Я Алексей, мой любимый цвет — #0000FF.\n");
Пример решения через Sublime Text + Ubuntu:
Создайте файл about_me.c.

Напишите код:

c
Copy
#include <stdio.h>

int main() {
    printf("Меня зовут Анна, обожаю тёмно-фиолетовый (#2E0854)!\n");
    return 0;
}
Скомпилируйте и запустите:

bash
Copy
gcc about_me.c -o about_me && ./about_me
Советы для Ubuntu:
Горячие клавиши в терминале:

Ctrl + Shift + T → новый таб терминала.

↑/↓ → история команд.

Tab → автодополнение имён файлов.

Шорткаты Sublime Text:

Ctrl + S → сохранить.

Ctrl + B → собрать проект (если настроена система сборки).

Если возникнут проблемы:
Ошибка компиляции: Внимательно читайте сообщения — они укажут на строку с ошибкой.

Файл не запускается: Убедитесь, что вы дали права на выполнение:

bash
Copy
chmod +x hello
Когда напишете код, отправьте его мне, и я проверю! 💬
Вопросы есть? Спрашивайте, если что-то непонятно в настройке Sublime Text или работе с терминалом.
