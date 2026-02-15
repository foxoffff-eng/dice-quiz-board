# GitHub Pages Deploy

## 1. Создай пустой репозиторий на GitHub
- Пример: `https://github.com/<username>/dice-quiz-board`

## 2. Выполни команды в `P:\123`
```powershell
git init
git branch -M main
git add index.html
git add manifest.webmanifest
git add service-worker.js
git add icon-192.png
git add icon-512.png
git add icon-maskable-512.png
git add apple-touch-icon.png
git add .github/workflows/pages.yml
git add DEPLOY_GITHUB_PAGES.md
git commit -m "Deploy Dice Quiz to GitHub Pages"
git remote add origin https://github.com/<username>/dice-quiz-board.git
git push -u origin main
```

## 3. Включи Pages один раз
1. Открой `Settings -> Pages` в репозитории.
2. В `Source` выбери `GitHub Actions`.

## 4. Получи ссылку
- После пуша открой `Actions`, дождись workflow `Deploy Dice Quiz to GitHub Pages`.
- Сайт будет доступен по URL вида:
`https://<username>.github.io/dice-quiz-board/`

## Обновление сайта
- Меняешь `index.html`/`manifest.webmanifest`/`service-worker.js`.
- Делаешь `git add`, `git commit`, `git push`.
- GitHub Pages обновится автоматически.
