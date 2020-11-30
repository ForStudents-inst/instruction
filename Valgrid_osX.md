# instruction

Установка valgrind с помощью conda (os X)
-----

 Скачать  miniconda: 

    get http://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
 Запуск установки
 
    sh Miniconda3-latest-MacOSX-x86_64.sh
 Повяиться диалог:
 
    >Welcome to Miniconda3 py38_4.9.2
    >In order to continue the installation process, please review the license
    >agreement.
    >Please, press ENTER to continue
 Нажать ENTER
 
 Пролистать лицензию до конца, стрелками вниз

    >Do you accept the license terms? [yes|no]
 Ввести "yes"

    >Miniconda3 will now be installed into this location:
    >/Users/username/miniconda3
    >- Press ENTER to confirm the location
    >- Press CTRL-C to abort the installation
    >- Or specify a different location below
Ввести  новый путь, куда будет установлена miniconda, или согласится с выбранным

    >Do you wish the installer to initialize Miniconda3
    by running conda init? [yes|no]
Ввести "no"

Запуск переменных окружения conda
    
    >source path-to-miniconda/etc/profile.d/conda.sh
Добавление канала, в котором есть valgrind 
 
    >conda config --add channels conda-forge
Создание переменных окружения с valgrind
    
    >conda create --name val-env valgrind
    >Proceed ([y]/n)? 
Ввести "y"

Использование
-----
Запуск переменных окружения conda
    
    >source path-to-miniconda/etc/profile.d/conda.sh

Активация переменных окружения с valgrind

    > conda activate val-env
    
Деактивация перменных окружения после завершения работы с valgrind

    > conda deactivate

