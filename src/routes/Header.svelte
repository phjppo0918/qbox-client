<script>
    import Button, {Label} from "@smui/button";

    import TopAppBar, {
        Row,
        Section,
        Title,
        AutoAdjust,
    } from '@smui/top-app-bar';
    import IconButton from '@smui/icon-button';

    let topAppBar;
</script>


<Button color="secondary" variant="raised">
    <Label>signin</Label>
</Button>

<TopAppBar bind:this={topAppBar} variant="short">
    <Row>
        <Section>
            <Title>QBOX</Title>
        </Section>
        <Section align="end">
            <Button variant="raised">
                <Label>signup</Label>
            </Button>
            <Button color="secondary" variant="raised">
                <Label>signin</Label>
            </Button>
        </Section>
    </Row>
</TopAppBar>
<AutoAdjust {topAppBar}>

</AutoAdjust>

<style>
    /* Hide everything above this component. */
    :global(#smui-app),
    :global(body),
    :global(html) {
        display: block !important;
        height: auto !important;
        width: auto !important;
        position: static !important;
    }
</style>