<script lang="ts" setup></script>

<template>
    <div class="search-container">
        <h1 class="title">Search People</h1>

        <div class="search-container__input">
            <input type="text" v-model="query" />
            <button @click="search">Search</button>
        </div>

        <div class="search-container__results">
            <div class="search-result" v-for="person in results">
                <h3 class="search-result__name">{{ person.name }}</h3>
                <div class="search-result__portrait">
                    <img :src="person.image">
                </div>
                <p class="search-result__desc">{{ person.major }}</p>
                <p class="search-result__desc">{{ person.classification }}</p>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "SearchComponent",
    data() {
        return {
            query: "",
            results: []
        }
    },
    methods: {
        async search() {
            const options = {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({ year: 2023, query: this.query })
            };

            try {
                const response = await fetch('https://5tlzzz9460.execute-api.us-east-2.amazonaws.com/default/search-v2', options);
                const { people } = await response.json();
                this.results = people;
            } catch (e) {
                console.error(e instanceof Error && e.message);
            }
        },
    }
}
</script>

<style scoped></style>
