<template>
    <div class="mt-5">
        <b-button variant="danger">texto</b-button>
        <b-button variant="info">texto</b-button>
        <b-button variant="success">texto</b-button>
        <b-button variant="warning">texto</b-button>
        <b-button variant="primary">texto</b-button>
        <b-button variant="dark">texto</b-button>

        <b-row class="mt-5">
            <b-col cols="12" md="4">
                <b-card
                    title="Flowers"
                    img-src="https://picsum.photos/400/200/?image=25"
                    img-alt="Image"
                    tag="article"
                    style="max-width: 10rem;">
                    <p>
                        frase hermosa
                    </p>
                    <b-button href="#" variant="primary" >Go</b-button>

                </b-card>
            </b-col>
            <b-col cols="12" md="4">
                <b-card
                    title="Flowers"
                    img-src="https://picsum.photos/400/200/?image=25"
                    img-alt="Image"
                    tag="article"
                    style="max-width: 10rem;">
                    <p>
                        frase hermosa
                    </p>
                    <b-button href="#" variant="primary" >Go</b-button>

                </b-card>
            </b-col>
            <b-col cols="12" md="4">
                <b-card
                    title="Flowers"
                    img-src="https://picsum.photos/400/200/?image=25"
                    img-alt="Image"
                    tag="article"
                    style="max-width: 10rem;">
                    <p>
                        frase hermosa
                    </p>
                    <b-button href="#" variant="primary" >Go</b-button>

                </b-card>
            </b-col>
        </b-row>
        
       
    </div>
</template>

<script>
export default({
   name: 'Card'
})
</script>
