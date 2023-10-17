<script>
    import DataTable, {Head, Body, Row, Cell} from '@smui/data-table';
    import LinearProgress from '@smui/linear-progress';
</script>

<h1>질문 목록</h1>

<DataTable table$aria-label="User list" style="width: 100%;">
    <Head>
        <Row>
            <Cell numeric>ID</Cell>
            <Cell style="width: 100%;">제목</Cell>
            <Cell>작성자</Cell>
            <Cell>댓글 수</Cell>
        </Row>
    </Head>
    <Body>

    <Row>
        <Cell numeric>1</Cell>
        <Cell>홍길동</Cell>
        <Cell>가나다</Cell>
        <Cell numeric>4</Cell>
    </Row>
    <Row>
        <Cell numeric>1</Cell>
        <Cell>홍길동</Cell>
        <Cell>가나다</Cell>
        <Cell numeric>4</Cell>
    </Row>
    <Row>
        <Cell numeric>1</Cell>
        <Cell>홍길동</Cell>
        <Cell>가나다</Cell>
        <Cell numeric>4</Cell>
    </Row>

    </Body>

    <LinearProgress
            indeterminate
            aria-label="Data is being loaded..."
            slot="progress"
    />
</DataTable>


<style>

</style>