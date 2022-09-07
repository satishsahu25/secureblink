<template>
    <div class="numbers">
        <div>
            <h4>Total Students</h4>
            <span>5140</span>
        </div>
        <div>
            <h4>Partners</h4>
            <span>4120</span>
        </div>
        <div>
            <h4>Affliate Distribution</h4>
            <span>4.18Lac</span>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

.numbers{
    margin-top: 8rem;
    margin-bottom:8rem;
    display: flex;
    justify-content: space-around;
}

.numbers h4{
    color: #86919D;
    font-size: 25px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
.numbers div span{
    font-weight: 700;
    font-size: 40px;
    border-bottom: 5px solid #01CB63;
}

@media only screen and (max-width: 760px) {
        .numbers{
            flex-direction: column;
            align-items: center;
            text-align: center;
        }
        .numbers div{
            margin-top: 1rem;
        }
    }
</style>