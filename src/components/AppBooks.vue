<script>
    export default{
        name: 'AppBooks',
    }
</script>

<template>
    <div id="books-comic">
        <div id="container-books">
            <button>Current series</button>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit non ut amet corporis nam delectus id consequatur explicabo accusantium obcaecati, alias cupiditate quam consectetur unde in nostrum laboriosam maiores quae!</p>
        </div>
        
    </div>
</template>

<style lang="scss">
    @use '../styles/variables' as *;

    #books-comic{
        height: 670px;
        width: 100%;
        background-color: #1c1c1c;

        button{
            position: relative;
            top: -25px;
            left: -20px;
            background-color: $primaryColorBlue;
            padding: 10px 30px;
            border: transparent;
            font-size: 25px;
            text-transform: uppercase;
            font-weight: bold;
        }

        #container-books{
            width: 1250px;
            margin: 0 auto;
        }
    }
</style>