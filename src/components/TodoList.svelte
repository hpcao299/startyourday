<div class="note-paper">
    <div class="pin"></div>
    <div class="note-content">
        <h2>To-do list</h2>
        <ul class="todos">
            <li class="todo-item">
                <label for="">
                    <input type="checkbox" />
                    <span>Finish the task</span>
                </label>
            </li>
            <li class="todo-item">
                <label for="">
                    <input type="checkbox" />
                    <span>Finish the task</span>
                </label>
            </li>
            <li class="todo-item">
                <label for="">
                    <input type="checkbox" />
                    <span>Finish the task</span>
                </label>
            </li>
        </ul>
    </div>
</div>

<style>
    .note-paper {
        background-color: #fffbba;
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 20px;
        width: 100%;
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
        font-size: 20px;
        text-align: center;
    }

    .note-content {
        font-size: 14px;
        line-height: 1.5;
    }

    .todos {
        list-style-type: none;
        margin-top: 20px;
        padding: 0 8px;
    }

    .todo-item {
        padding: 12px 0;
    }

    .todo-item:not(:last-child) {
        border-bottom: 1px solid #ccc;
    }

    .todo-item label {
        display: flex;
        align-items: center;
    }

    .todo-item span {
        font-size: 18px;
    }

    .todo-item input {
        margin-right: 8px;
        width: 15px;
        height: 15px;
    }

    .todo-item input:checked ~ span {
        text-decoration: line-through;
    }
</style>
