<template>
    <div class="mt-5">
        <form action="">
            <b-row>
                <b-col md="3">
                    <b-form-input type="number" v-model="texto" :state="comprobando"></b-form-input>
                    <small> Minimo 3 caracteres</small>
                    <p>Texto: {{texto}}</p>
                </b-col>
                <b-col md="3">
                    <b-form-select v-model="select" :options="animal"></b-form-select>
                    <p>Seleccionaste un: {{select}}</p>
                </b-col>
                <b-col md="3">
                    <b-form-radio-group v-model="radio" :options="animalRadio"></b-form-radio-group>
                    <p>animal: {{radio}}</p>
                </b-col>
                <b-col md="3">
                    <b-form-checkbox-group v-model="check" :options="animalRadio"></b-form-checkbox-group>
                     <p>Multiples: {{check}}</p>
                </b-col>
            </b-row> 
        </form>
        

    </div>
</template>

<script>
export default {
    name: 'Form',
    data() {
        return {
            texto: '',
            select: null,
            radio: 'Gato',
            check: ['Gato'],
            animal: [
                {value: null, text: 'Seleccione un aminal'},
                {value: 'Gato', text: 'Peludo y jugueton'},
                {value: 'Perro', text: 'Travieso y amoroso'},
                {value: 'Oso', text: 'Salvaje y Fuerte'}
            ],
            animalRadio: [
                {value: 'Gato', text: 'Peludo y jugueton'},
                {value: 'Perro', text: 'Travieso y amoroso'},
                {value: 'Oso', text: 'Salvaje y Fuerte'}
            ],
        };
    },
    computed:{
        comprobando(){
            return this.texto.length >2 ?true: false;
        }
    }
}
</script>