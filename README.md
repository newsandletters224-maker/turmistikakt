# Тұрғын үй жағдайын тексеру актісі

Веб-қосымша — әлеуметтік қызметкерлерге арналған құрал. Тұрғын үй-тұрмыстық жағдайды тексеру актісін Word (.docx) форматында жасауға мүмкіндік береді.

## Мүмкіндіктер

- 📝 Қазақ тілінде интерфейс
- 🔒 Толық құпиялылық — деректер тек браузерде өңделеді
- 📄 Word (.docx) құжатын автоматты түрде жасау
- 📱 Адаптивті дизайн (ноутбук, планшет)
- ✅ Валидация — міндетті өрістерді тексеру
- 🗑️ Форманы тазалау мүмкіндігі

## Құпиялылық

- Ешқандай backend, база данных немесе API жоқ
- Деректер localStorage/sessionStorage/cookies-те сақталмайды
- Word құжаты толығымен браузерде (client-side) жасалады
- Аналитика, логирование, трекерлер жоқ

## Локалды іске қосу

```bash
npm install
npm run dev
```

Браузерде `http://localhost:3000` ашылады.

## Build

```bash
npm run build
```

Нәтиже `dist/` папкасында болады.

## Deploy

### Vercel

1. GitHub-қа кодты пуш етіңіз
2. [vercel.com](https://vercel.com) сайтында "New Project" → GitHub репозиторийін таңдаңыз
3. Framework Preset: Vite
4. "Deploy" басыңыз

### Render

1. GitHub-қа кодты пуш етіңіз
2. [render.com](https://render.com) сайтында "New Static Site" → репозиторийді таңдаңыз
3. Build Command: `npm run build`
4. Publish Directory: `dist`
5. "Create Static Site" басыңыз

## Технологиялар

- React 18 + TypeScript
- Vite
- Tailwind CSS 4
- docx (Word құжатын жасау)
- file-saver (файлды жүктеу)

## Құрылым

```
src/
├── App.tsx              # Негізгі компонент (форма)
├── types.ts             # TypeScript типтері
├── utils/
│   └── generateDocument.ts  # Word құжатын жасау логикасы
├── main.tsx             # Қосымшаның кіру нүктесі
└── index.css            # Стильдер
```
