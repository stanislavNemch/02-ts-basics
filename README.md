# Feedback Widget (Віджет відгуків)

Це простий, але функціональний віджет для збору відгуків, створений за допомогою React та TypeScript. Користувачі можуть оцінити сервіс, обравши один із трьох варіантів ("Добре", "Нейтрально", "Погано"), і миттєво побачити оновлену статистику.

Цей проєкт є чудовою практикою для початківців, щоб зрозуміти ключові концепції React, такі як керування станом, передача пропсів та умовний рендеринг, а також основи типізації в TypeScript.

---

## 🇺🇦 Українська версія

### ✨ Технології та стек

-   **React**: бібліотека для створення динамічних користувацьких інтерфейсів.
-   **TypeScript**: додає статичну типізацію до JavaScript, що робить код надійнішим.
-   **Vite**: сучасний та швидкий інструмент для збирання проєктів.
-   **CSS Modules**: для локальної стилізації компонентів, що запобігає конфліктам імен класів.
-   **Modern-normalize**: для скидання та нормалізації стилів браузера.

### 📂 Структура проєкту

Проєкт має чітку компонентну структуру, що полегшує його розуміння та масштабування.

```
/src
|-- /components     # Директорія з усіма компонентами
|   |-- /App        # Головний компонент-контейнер
|   |-- /CafeInfo   # Компонент з інформацією про кафе
|   |-- /Notification # Компонент для сповіщень
|   |-- /VoteOptions  # Компонент з кнопками для голосування
|   |-- /VoteStats    # Компонент для відображення статистики
|-- /types          # Директорія для загальних типів TypeScript
|   |-- votes.ts    # Типи, пов'язані з голосуванням
|-- main.tsx        # Вхідна точка додатку
```

\#\#\#🎯 Основні моменти для початківця

При розробці цього проєкту основний фокус був на наступних аспектах:

1.  **Керування станом**: використання хука `useState` для зберігання та оновлення кількості голосів. Стан централізовано в головному компоненті `App`.
2.  **Композиція компонентів**: додаток зібрано з невеликих, незалежних компонентів (`CafeInfo`, `VoteOptions`, `VoteStats`), що робить код чистішим і легшим для підтримки.
3.  **Передача даних через пропси**: дочірні компоненти отримують дані та функції для керування станом від батьківського компонента `App`.
4.  **Умовний рендеринг**: компонент `VoteStats` відображається, лише якщо є хоча б один відгук. В іншому випадку показується `Notification`. Кнопка "Reset" також з'являється за умовою.
5.  **Основи TypeScript**: застосування інтерфейсів (`interface`) та типів (`type`) для типізації пропсів та стану, що підвищує надійність коду.

---

## 🇬🇧 English Version

### ✨ Technologies & Stack

-   **React**: A library for building dynamic user interfaces.
-   **TypeScript**: Adds static typing to JavaScript, making the code more robust.
-   **Vite**: A modern and fast build tool for web projects.
-   **CSS Modules**: For locally scoped component styling to prevent class name conflicts.
-   **Modern-normalize**: For resetting and normalizing browser styles.

### 📂 Project Structure

The project has a clear component-based structure, making it easy to understand and scale.

```
/src
|-- /components     # Directory for all components
|   |-- /App        # Main container component
|   |-- /CafeInfo   # Component with cafe information
|   |-- /Notification # Component for notifications
|   |-- /VoteOptions  # Component with voting buttons
|   |-- /VoteStats    # Component for displaying statistics
|-- /types          # Directory for shared TypeScript types
|   |-- votes.ts    # Types related to votes
|-- main.tsx        # Application entry point
```

### 🎯 Key Focus Points for a Beginner

While developing this project, the main focus was on the following aspects:

1.  **State Management**: Using the `useState` hook to store and update the vote counts. The state is centralized in the main `App` component.
2.  **Component Composition**: The application is built from small, independent components (`CafeInfo`, `VoteOptions`, `VoteStats`), which makes the code cleaner and easier to maintain.
3.  **Passing Data via Props**: Child components receive data and state management functions from the parent `App` component.
4.  **Conditional Rendering**: The `VoteStats` component is rendered only if there is at least one vote. Otherwise, the `Notification` component is displayed. The "Reset" button also appears conditionally.
5.  **TypeScript Basics**: Applying interfaces and types to type-check props and state, which improves code reliability.
