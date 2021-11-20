<template>
  <button 
  @click="onClick('value')"
  :style="[ spanX < 2 || spanY < 2 ? {width: '45px' } :{width: '92px'}]"
 
  class="btn"
  >{{  value }}
  </button>

  <!-- =" this.spanX < 0 ? {width: 
   this.spanX = 1 * Math.trunc((this.const * Math.trunc(this.spanX) )) + (2 *( Math.trunc(this.spanX) -1))+'px' }
  ]" -->

    <!-- :style="[ spanX = 1  ?  {'width: 45px'} : {'width: 190px'} ]" -->


</template>

//   :style="{background: const}"


<script>
 

export default {

  

    props: {
        value:String,
        // eslint-disable-next-line no-global-assign
        
        const: {
            type:Number,
            default:45
        },

        spanX: {
            type:Number,
            default: 1 ,
        },
        
        spanY: {
            type:Number,
            default: 1} ,
        
        color: {
            type:String,
            default:'gray'
        }
        ,
        // eslint-disable-next-line no-global-assign
        // ancho:document.getElementById("value").style.backgroundColor,
    },
    computed: {
        resultQ () {
                   // eslint-disable-next-line vue/no-side-effects-in-computed-properties
                   return this.spanx = Math.trunc(this.spanx ) 
        },
    },

    methods: {
        onClick() {
            console.log( 'spanX = ', this.spanX ,   'value: ', this.value, 
            'spanY = ', this.spanY
            );
            //  document.documentElement.style.setProperty('--ancho', this.const + 'px');
        }
    },
   

}
</script>

<style>
:root {
    --somevar: blue;
    --ancho: 45px;
    --alto:45px
}

.btn {
    font-size: 40px;
    font-weight: bold;
    margin: 2px;
    /* background: var(--somevar); */
    width: var(--ancho);
    height: var(--alto);
}

</style>