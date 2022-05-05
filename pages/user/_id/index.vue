<template>
    <h2>Welcome : {{$route.params.id}}</h2>
</template>


<script>
import { defineComponent } from '@vue/composition-api'

export default ({
    validate(data) {
        return /^\d+$/.test(data.params.id)
    },
})
</script>
