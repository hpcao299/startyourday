<script lang="ts"></script>

<div class="content">
    <div class="note-paper">
        <div class="pin"></div>
        <div class="note-content">
            <h2>Note Title</h2>
            <p>This is a sample note content. You can add your own content here.</p>
        </div>
    </div>
</div>

<style>
    .note-paper {
        background-color: #fffbba;
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 20px;
        width: 300px;
        position: relative;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .pin {
        width: 20px;
        height: 20px;
        background-color: #999;
        border-radius: 50%;
        position: absolute;
        top: -10px;
        left: calc(50% - 10px);
        transform: rotate(-45deg);
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    }

    .pin::before {
        content: '';
        width: 2px;
        height: 10px;
        background-color: #999;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .note-paper h2 {
        font-weight: 700;
    }

    .note-content {
        font-size: 14px;
        line-height: 1.5;
    }
</style>
