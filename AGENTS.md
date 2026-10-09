<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Keep greeting data frontend-only in a browser-safe data module holding the class roster; this avoids a database, backend and recipient authentication while staying transform-safe.
- Export the rendered greeting with html-to-image after fonts load; this keeps downloaded cards consistent with the visible card.
- Keep greeting styles and button variants in the global semantic design system; this ensures one consistent visual language.
- Define card templates in a browser-safe registry and render all templates through the shared GreetingCard; this preserves recipient data and keeps selection and PNG export on one rendering path.
