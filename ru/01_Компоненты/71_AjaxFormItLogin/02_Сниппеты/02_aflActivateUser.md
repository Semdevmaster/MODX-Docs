# AjaxFormitLogin

Сниппет активации аккаунта пользователя. Если ссылка активации просрочена - профиль будет удалён.

Этот сниппет не принимает никаких параметров.

## Пример использования

```html
{set $user  = '!aflActivateUser' | snippet:[]}
{if $user}
<h2>Уважаемый, {$user.username}, Ваш аккаунт успешно активирован!</h2>
{/if}
```

В случае успешной активации будет возвращён массив со всеми данными пользователя, если активация будет неудачной - вернётся false.
