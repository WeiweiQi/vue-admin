<template>
    <el-input 
        v-model="model" 
        v-bind="$attrs"
        type="password"
    ></el-input>
</template>

<script lang="ts">
import { Vue, Component} from 'vue-property-decorator'

import _props_value_mixin from "./_props_value_mixin"
import _computed_model_mixin from "./_computed_model_mixin"

@Component({
    name:"field_pwd",
    inheritAttrs:true,
    mixins:[
        _props_value_mixin,
        _computed_model_mixin,
    ],
})
export default class field_pwd extends Vue{

}
</script>