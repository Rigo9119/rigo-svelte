<script>
    const nd = new Date();
    const day = nd.getDate();
    const month = nd.toLocaleString('default', { month: 'long' });
    const year = nd.getFullYear()
    const date = `${year} / ${month.toUpperCase()} / ${day} `;
</script>

<footer class="footer">
    <p class="footer__message">
        Made with SvelteKit by Rigo Rosero C
        <span class="footer__date">{date}</span>
    </p>
</footer>

<style lang="scss">
    .footer {
        align-items: center;
        align-self: flex-end;
        display: flex;
        justify-content: center;
        padding: 22px 0;
        &__message {}

        &__date {
            font-style: italic;
        }
    }
</style>
