<template>
    <div class="max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8">
        <h1
            class="py-4 text-3xl leading-9 tracking-tight font-extrabold text-gray-900 sm:text-4xl sm:leading-10"
        >
            Sponsors
        </h1>
        <div class="cards-grid py-2">
            <SponsorCard>
                <template #image>
                    <a href="https://tailwindcss.com">
                        <img
                            class="h-10"
                            src="/img/logos/tailwindcss-logo.svg"
                            alt="tailwindcss"
                        />
                    </a>
                </template>
                <p class="text-lg text-grey-600">
                    Thanks to
                    <a
                        class="text-brand-primary underline"
                        href="https://tailwindcss.com"
                        >Tailwind CSS</a
                    >
                    for providing a team account for
                    <a
                        class="text-brand-primary underline"
                        href="https://tailwindui.com"
                        >Tailwind UI</a
                    >
                    which we used to help develop this site.
                </p>
            </SponsorCard>
            <SponsorCard>
                <template #image>
                    <a href="https://1password.com/">
                        <img
                            class="h-10"
                            src="/img/logos/1P-wordmark.svg"
                            alt="1 Password"
                        />
                    </a>
                </template>
                <p class="text-lg text-grey-600">
                    Thanks to
                    <a
                        class="text-brand-primary underline"
                        href="https://1password.com/"
                        >1Password</a
                    >
                    for providing a team account for DES members to manage our
                    passwords.
                </p>
            </SponsorCard>
            <SponsorCard>
                <template #image>
                    <a href="https://shortcut.com/">
                        <img
                            class="h-10"
                            src="/img/logos/Shortcut_full_color.svg"
                            alt="shortcut"
                        />
                    </a>
                </template>
                <p class="text-lg text-grey-600">
                    Thanks to
                    <a
                        class="text-brand-primary underline"
                        href="https://shortcut.com/"
                        >Shortcut.</a
                    >
                    The project management platform we use to help organise our
                    team.
                </p>
            </SponsorCard>
        </div>
    </div>
</template>

<script>
import SponsorCard from "../components/SponsorCard";
export default {
    components: {
        SponsorCard,
    },
};
</script>

<style>
.cards-grid {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    justify-items: center;
}
</style>
