# Шрифт MorfinSans

Положите сюда файлы шрифта, чтобы он заработал на сайте:

- `MorfinSans.woff2` — основной формат (быстрее грузится)
- `MorfinSans.ttf` — резервный формат

Сайт уже ссылается на эти пути в `@font-face`:

```css
@font-face {
  font-family: 'MorfinSans';
  src: url('fonts/MorfinSans.woff2') format('woff2'),
       url('fonts/MorfinSans.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}
```

## Где взять

MorfinSans — коммерческий шрифт. Варианты:

1. **Купить лицензию** у автора/на шрифтовом маркетплейсе (MyFonts, Creative Market).
2. **Найти бесплатный аналог** с похожим характером:
   - **Cormorant Garamond** — уже подключён как fallback, работает прямо сейчас
   - **Playfair Display** — более контрастный
   - **Marcellus** — строгий антиквенный

## Пока файлов нет

Сайт автоматически использует fallback из CSS:
`font-family: 'MorfinSans', 'Cormorant Garamond', sans-serif;`

То есть заголовки уже выглядят прилично на Cormorant Garamond.
Как только положите файлы в эту папку — MorfinSans подхватится сам, без правок кода.
