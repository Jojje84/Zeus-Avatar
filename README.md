# Zeus Avatar Lab

En lätt prototyp för en animerad Zeus-avatar som kan köras direkt i webbläsaren och senare på en Raspberry Pi.

## Tre karaktärer

- **Den vise** – varm, lugn äldre man
- **Olympiern** – tydligare Zeus/gud-känsla
- **Professorn** – modern äldre mentor med glasögon

## Fyra lägen

- `idle`
- `listening`
- `thinking`
- `speaking`

Prototypen använder bara HTML, CSS, SVG och JavaScript. Inga externa bibliotek krävs.

## Styra från Zeus senare

```js
ZeusAvatar.setState("listening")
ZeusAvatar.setState("thinking")
ZeusAvatar.setState("speaking")
ZeusAvatar.setState("idle")

ZeusAvatar.setCharacter("wise")
ZeusAvatar.setCharacter("olympian")
ZeusAvatar.setCharacter("professor")
```

Nästa steg är att koppla detta till Zeus backend via WebSocket eller SSE så att avataren reagerar automatiskt på Zeus riktiga status.

## GitHub Pages

Repo:t innehåller ett GitHub Actions-workflow för Pages. Om Pages inte redan är aktiverat, välj **Settings → Pages → Source: GitHub Actions** en gång. Därefter deployas sidan automatiskt vid push till `main`.
