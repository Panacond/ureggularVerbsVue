<script>
export default {
    props: ['word', 'index'],
    computed: {
        showExamlpe() {
            if (this.word.example.length > 0)
                return "add";
        },
        show() {
            if (this.word.example.length > 0)
                return true;
        }
    },}
</script>
<template>
    <div :class="showExamlpe">
            <div>
                <div>{{ index + 1 }}</div>
                <div>{{word.word[0]}}</div>
                <div>{{word.word[1]}}</div>
                <div>{{word.word[2]}}</div>
                <div>{{word.translate}}</div>
            </div>
            <div v-show="show">
                <ul>
                    <li v-for="(i) in word.example">
                        {{i}}
                    </li>
                </ul>
            </div>
        </div>
</template>