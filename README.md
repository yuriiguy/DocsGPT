<h1 align="center">
  DocsGPT  🦖
</h1>

<p align="center">
  <strong>Помічник з документації з відкритим кодом</strong>
</p>

<p align="left">
  <strong>DocsGPT</strong> це передове рішення з відкритим кодом, яке спрощує процес пошуку інформації в проектній документації. Завдяки інтеграції потужних моделей <strong>GPT</strong> розробники можуть легко ставити запитання про проект і отримувати точні відповіді.
  
Попрощайтеся з трудомістким ручним пошуком і дозвольте <strong>DocsGPT</strong> допомогти вам швидко знайти потрібну інформацію. Спробуйте й подивіться, як це революціонізує ваш досвід проектної документації. Внесіть свій внесок у його розвиток і станьте частиною майбутнього допомоги на основі ШІ.
</p>

<div align="center">
  
  <a href="https://discord.gg/n5BX8dh8rU">![example1](https://img.shields.io/github/stars/arc53/docsgpt?style=social)</a>
  <a href="https://discord.gg/n5BX8dh8rU">![example2](https://img.shields.io/github/forks/arc53/docsgpt?style=social)</a>
  <a href="https://discord.gg/n5BX8dh8rU">![example3](https://img.shields.io/github/license/arc53/docsgpt)</a>
  <a href="https://discord.gg/n5BX8dh8rU">![example3](https://img.shields.io/discord/1070046503302877216)</a>
  
</div>

![video-example-of-docs-gpt](https://d3dg1063dc54p9.cloudfront.net/videos/demov3.gif)


## Oсобливості

![Group 9](https://user-images.githubusercontent.com/17906039/220427472-2644cff4-7666-46a5-819f-fc4a521f63c7.png)

## Дорожня карта

Ви можете знайти нашу [Roadmap](https://github.com/orgs/arc53/projects/2) тут, будь ласка, не соромтеся робити внески або створювати проблеми, це допоможе нам покращити DocsGPT!



## [Live preview](https://docsgpt.arc53.com/)

## [Приєднуйтесь до нашого Discord](https://discord.gg/n5BX8dh8rU)


## Структура проекту
- Application - програма flask (основна програма)

- Extensions - розширення chrome

- Scripts - сценарій, який створює індекс пошуку подібності та зберігає для інших бібліотек. 

- frontend - інтерфейс in vite and

## Швидкий початок

Примітка. Переконайтеся, що докер встановлено

1. Відкрийте завантажте це сховище за допомогою `git clone https://github.com/arc53/DocsGPT.git`
2. Відкрийте docker-compose.yaml і замініть <your_api_key> на ваш ключ OpenAI (є 4 місця)
3. Запустіть `docker-compose build && docker-compose up`

Щоб зупинитися, просто запустіть Ctrl + C

## Середовища розробки

Розгорнути лише 2 контейнери з docker-compose.yaml (видаливши всі служби, крім redis і mongo)

Переконайтеся, що у вас встановлено python 3.10 або 3.11

1. Перейдіть до папки `/application`
2. Встановити залежності `pip install -r requirements.txt`
3. Підготуйте файл .env
Скопіюйте .env_sample і створіть .env за допомогою токена openai API
4. Запустіть програму `python app.py`
5. Почніть робщту з `celery -A app.celery worker -l INFO`

Щоб запустити інтерфейс:
1. Navigate to `/frontend` folder
2. Install dependencies
`npm install`
3. In the file  `.env.development` instead of `VITE_API_HOST = https://docsapi.arc53.com` use `VITE_API_HOST=http://localhost:5001`
3. Run the app
4. `npm run dev`


[Як встановити розширення Chrome?](https://github.com/arc53/docsgpt/wiki#launch-chrome-extension)


## [Посібники](https://github.com/arc53/docsgpt/wiki)

## [Хочете зробити внесок?](https://github.com/arc53/DocsGPT/blob/main/CONTRIBUTING.md)

## [Як використовувати будь-яку іншу документацію](https://github.com/arc53/docsgpt/wiki/How-to-train-on-other-documentation)

## [Як розмістити його локально (щоб усі дані залишалися на місці)](https://github.com/arc53/DocsGPT/wiki/How-to-use-different-LLM's#hosting-everything-locally)

Побудований [🦜️🔗 LangChain](https://github.com/hwchase17/langchain)
