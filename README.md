
# Outrun — аркадная гоночная игра

## Обзор
Outrun — это простая аркадная гоночная игра, вдохновлённая классическими ретро-гонками. Игра реализована на C++ с использованием библиотеки SFML. Игрок управляет автомобилем, который движется по извилистой трассе с различными препятствиями и объектами на дороге. Основная цель — проехать как можно дальше, избегая столкновений и не вылетая с трассы.

В игре реализована псевдо-3D перспектива, плавные повороты, смена высоты дороги и разнообразные объекты вдоль трассы (деревья, столбы, здания и т.д.). Управление осуществляется с помощью клавиш-стрелок: влево/вправо — повороты, вверх/вниз — ускорение и замедление. Игра отлично подходит для демонстрации работы с графикой и анимацией в SFML.

## Структура проекта
Наш проект состоит из следующих файлов и папок:

- **.github/workflows/**: Содержит файлы конфигурации GitHub Actions для сборки проекта на разных платформах.
  - **build-linux.yml**: Конфигурация для сборки проекта в среде Linux с использованием Clang.
  - **build-windows.yml**: Конфигурация для сборки проекта в среде Windows.

- **src/**: Содержит исходный код игры.
  - **main.cpp**: Точка входа в приложение, инициализация игры и запуск игрового цикла.
  - **game.cpp**: Реализация игровой логики, включая обновление состояния и рендеринг.
  - **game.h**: Заголовочный файл, содержащий объявления классов и функций, используемых в game.cpp.

- **CMakeLists.txt**: Конфигурационный файл для CMake, задающий имя проекта, требуемый стандарт C++ и исходные файлы.

- **README.md**: Документация проекта, включая инструкции по сборке и запуску.

- **LICENSE**: Лицензионная информация о проекте.

## Инструкции по сборке

### Linux
1. Убедитесь, что на вашей системе установлены Clang и CMake.
2. Клонируйте репозиторий на локальный компьютер.
3. Перейдите в директорию проекта.
4. Выполните следующие команды для сборки проекта:
   ```bash
   mkdir build
   cd build
   cmake ..
   make
   ```

### Windows
1. Убедитесь, что у вас установлен совместимый компилятор C++ и CMake.
2. Клонируйте репозиторий на локальный компьютер.
3. Перейдите в директорию проекта.
4. Выполните следующие команды для сборки проекта:
   ```cmd
   mkdir build
   cd build
   cmake ..
   cmake --build . --config Release
   ```

## Запуск игры
После сборки проекта вы можете запустить игру, выполнив скомпилированный бинарный файл:
- На Linux:
  ```bash
  ./Outrun
  ```
- На Windows:
  ```cmd
 Outrun.exe
  ```
