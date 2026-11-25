<script>
    import FileReader from "./file-reader.svelte";
    import DownloadTemplate from "./download-template.svelte";
</script>

<div class="titleBar">
    <div class="title">
        <h1 class="titleText">Impact tool</h1>
    </div>
    <div class="buttonGroup">
        <DownloadTemplate />
        <FileReader />
    </div>
</div>

<style>
    .titleBar {
        border-bottom: 1px solid black;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .title {
        display: flex;
        flex-direction: row;
    }

    .titleText {
        margin: 0;
        font-size: 40px;
        font-weight: 600;
        padding-top: 14px;
    }

    .buttonGroup {
        display: flex;
        align-items: center;
    }

    @media (max-width: 768px) {
        .titleBar {
            flex-direction: column;
            align-items: start;
        }
        
        .title {
            width: 100%;
            padding-bottom: 10px;
            border-bottom: 1px solid black;
            margin-bottom: 10px;
        }

        .buttonGroup {
            margin-left: 5px;
        }
    }
</style>