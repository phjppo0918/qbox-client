<script >
    import Card from "@smui/card";
</script>

<h1>강의 목록</h1>

<div class="card-display">
    <div class="card-container">
        <Card color="primary" variant="raised" padded>웹프로그래밍기초</Card>
    </div>
    <div class="card-container">
        <Card color="primary" variant="raised" padded>웹프로그래밍응용</Card>
    </div>
    <div class="card-container">
        <Card color="primary" variant="raised" padded>프로그래밍과데이터분석</Card>
    </div>
</div>


<style>
    .card-display {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 70vh;
        flex-direction: row;
        flex-wrap: wrap;
        align-content: space-around;
    }

    .card-container {
        height: 5vh;
        width: 80vw;
    }
</style>