# Референсы и find-skills

## Выбранный источник визуального направления

[Lavender Club](../visual-round-2/03-lavender-club.png) — сгенерированный для этого проекта концепт, выбранный пользователем. У него нет конкретного стороннего сайта-первоисточника. Палитра, типографический характер и иллюстрации этого изображения приоритетнее остальных галерей. Референсы ниже помогают решать детали, не меняя выбранное направление.

## Как использован запрошенный skill

Установлен и прочитан [find-skills / SKILL.md](../../.agents/skills/find-skills/SKILL.md) из [vercel-labs/skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills). В репозитории сохранён `skills-lock.json`.

Команда пользователя выполнена с явным проектным агентом и неинтерактивным флагом:

```bash
npx skills add vercel-labs/skills@find-skills --agent codex -y
```

Для среды использован отдельный npm cache в `/tmp`, поскольку стандартный каталог cache недоступен. Установка завершилась успешно; установленный текст совпал по SHA-256 с прочитанным официальным SKILL.md. Skill помогает найти специализированные инструкции, но сам не создаёт дизайн-систему.

По его процессу проверен [skills.sh](https://skills.sh/), выполнен `npx skills find "design system"`. Этот точный запрос не дал результатов. В leaderboard найдены подходящие кандидаты, проверены официальные репозитории и их GitHub stars. Числа — снимок 27 октября 2026 года, а не гарантия качества.

| Кандидат | Назначение для следующего этапа | Снимок источников |
|---|---|---|
| [anthropics/skills — frontend-design](https://skills.sh/anthropics/skills/frontend-design) | Цельное художественное направление и реализация интерфейса | Около 1,0 млн установок в leaderboard; репозиторий 184 137 stars |
| [vercel-labs/agent-skills — web-design-guidelines](https://skills.sh/vercel-labs/agent-skills/web-design-guidelines) | Аудит веб-интерфейса и доступности | Около 790,4 тыс. установок; репозиторий 33 092 stars |

Команды для будущего этапа: `npx skills add anthropics/skills@frontend-design` и `npx skills add vercel-labs/agent-skills@web-design-guidelines`. Эти дополнительные skills не устанавливались и их выполнение не заявляется. Их инструкции перед применением нужно прочитать. Текущая спецификация написана по выбранному изображению, изученным источникам и научной базе.

## Карта внешних источников

Полная таблица всех предоставленных URL, включая назначение и доступность: [UI_SOURCES.md](../research/UI_SOURCES.md). Сохраняем её как приложение к плану. Ниже указана роль групп именно для Lavender.

| Источники пользователя | Что берём / где применяем |
|---|---|
| [Dribbble](https://dribbble.com/search/language-learning-web-app), [Refero](https://refero.design), [Mobbin](https://mobbin.com/discover/apps/web/latest) | Сравнение учебных потоков, формы карточек, детализация компонентов. Конкретные закрытые экраны не считаются просмотренными. Dribbble при проверке вернул пустой ответ 202. |
| [Land-book](https://land-book.com), [Seesaw](https://www.seesaw.website), [Supahero](https://supahero.io) | Hero, масштаб иллюстрации и баланс текста, выбранная лавандовая эстетика сохраняется. |
| [Dark.design](https://www.dark.design), [Selected](https://selected.site), [Landing.love](https://www.landing.love), [Saaspo](https://saaspo.com), [BentoGrids](https://bentogrids.com) | Вторичная насмотренность. Не переносим тёмный стиль, тяжёлые эффекты и мозаику в фокусную тренировку. |
| [Navbar.gallery](https://www.navbar.gallery), [CTA.gallery](https://www.cta.gallery), [Footer.design](https://www.footer.design) | Навигация, понятное главное действие; футер нужен публичным страницам, не упражнению. |
| [60fps](https://60fps.design), [Motion](https://motion.dev) | Короткая обратная связь и reduced motion. Статичный снимок галереи не означает просмотр её видео. |
| [FontOfWeb](http://fontofweb.com), [Nitin Sangwan](https://nitinsangwan.com), [Boyare](https://boyare.su), [Telegram](https://t.me/boyaresu) | Типографическая насмотренность и оптический баланс. FontOfWeb перенаправляет на Fudge; Telegram отдельно не изучался. |
| [beUI](https://beui.dev), [BoardUI](https://www.boardui.com), [Uiverse](https://uiverse.io/elements), [Kokonut](https://kokonutui.com/docs/cards/card-flip) | Выборочные компоненты, адаптируемые к токенам Lavender. Проверить лицензию, клавиатуру и состояния; карточка раскрывается только явным действием. |
| [CanvasUI](https://canvasui.dev/components), [Particles](https://particles.casberry.in) | Не включаем GPU-эффекты в ядро обучения. |
| [xyflow](https://github.com/xyflow/xyflow) | Возможный будущий внутренний редактор; не зависимость MVP. |
| [Remotion](https://www.remotion.dev), [MotionSites](https://motionsites.ai), [Framer](https://www.framer.com), [GSAP](https://github.com/greensock/GSAP), [GSAP skills](https://github.com/greensock/gsap-skills), [OpenClaw Lovable](https://openclawmakeai.lovable.app) | Промо/дополнительные инструменты. Motion достаточен для выбранных интерфейсных переходов. OpenClaw-страница сейчас не подтверждает исходный видео-референс. |
| [skills.sh](https://skills.sh), [SkillsMP](https://skillsmp.com), [UI/UX Pro Max](https://skillsmp.com/skills/nextlevelbuilder-ui-ux-pro-max-skill-claude-skills-ui-ux-pro-max-skill-md), [design.md](https://design.md), [taste-skill](https://github.com/Leonxlnx/taste-skill) | Поиск/оценка инструкций для разработки. Не являются источником научных доказательств и не устанавливаются автоматически. |
| [Atlassian](https://atlassian.design), [Apple через DesignSystems.surf](https://designsystems.surf/design-systems/apple) | Семантика токенов, состояния, фокус, доступность и адаптация. Визуальный стиль остаётся Lavender. |
| [WebSnatch](https://www.websnatch.dev), SlicerDev `eeifohdpmcohfpmlbbanebcbpcncofhh`, [SVGLogo](https://svglogo.dev), [OwnYourCode](https://www.ownyourcode.dev), [Orca](https://www.onorca.dev), [Cursor MCP](https://cursor.directory/mcp) | Инструменты разработки, не функциональность ученика. Расширения не устанавливались, чужие компоненты не экспортировались. |

У Mobbin и Saaspo зафиксирован 403, у design.md — 503; HTML-оболочка некоторых галерей не позволяла изучить сами экраны. Selected.site и некоторые другие адреса изменили содержание. Эти ограничения сохраняются; новых заявлений о просмотре закрытых материалов план не делает.

Текстовые подборки о shadcn/Tailwind/Magic UI/Aceternity/Origin UI рассматриваются как возможные инструменты, а не обязательный набор зависимостей. Непредоставленные скриншоты чата и Google Doc о Stitch не анализировались. Для обучения команды freeCodeCamp полезен отдельно, но не задаёт продуктовую дизайн-систему.

## Научные и продуктовые источники

[База исследований](../../knowledge-base/vocabulary-learning/README.md) определяет учебные принципы и ограничения. [Официальная документация шести продуктов](../research/PRODUCTS.md) помогает проектировать сценарии. Галереи отвечают за визуальную насмотренность; их популярность и красивые экраны не доказывают эффективность запоминания.
