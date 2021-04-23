<script lang="ts">
    import Json from "./Json.svelte";

    export let json = {
        liste: [
            { hej: "med dig" },
            { med: "hej dig"},
            { dig: "og dine venner" }
        ],
        genstand: {
            hej: "med dig",
            med: "hej dig",
            dig: "og dine venner"
        },
        test: [ 1, 2, 3, 4],
        plop: { a: 10, b: 20, c: 30, d: "whatever" },
        answer: { q1: [ null, NaN ], q2: { quadratic: [ 1, null ] }, q3: [ "why", undefined ] }
    }

    import { foods } from './food-suggestions';
</script>

<main>
    <Json content={json}/>
    <Json content={foods}/>
</main>

<style>
    main {
        color: white;
    }
</style>