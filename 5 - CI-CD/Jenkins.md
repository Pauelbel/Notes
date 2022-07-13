## Установка 
* Скачать и установить [jenkins](https://www.jenkins.io/)
> Нужна java

## Настройки в Windows
* По умолчанию, ссылка для запуска главной страницы `http://localhost:8080/`


## Pipeline

### Declarative тип

Генератор pipeline из UI интерфейса доступен по ссылке [ссылка на наш jenkins](http://localhost:8080/pipeline-syntax/)
```groovy
pipeline {								- Директива													
    agent any							- Агент на котором запускается сборка
    stages {							- Этапы
        stage('Build') {				- Обязательный этап №1
            steps {						- Обязательный шаг
                echo 'Building..'		- Обязательный шаг
            }
        }
        stage('Test') {					- Обязательный этап №2
            steps {						- Обязательный шаг
                echo 'Testing..'		- Обязательный шаг
            }
        }
        stage('Deploy') {				- Обязательный этап №3
            steps { 					- Обязательный шаг
                echo 'Deploying....'	- Обязательный шаг
            }
        }
				
		post {                          - Определяет действия по завершению шага
			 always {
 			}
		}
    }
}
```
Ссылки:
[Неплохое видео](https://www.youtube.com/watch?v=oxbbnDpghCM)
 

