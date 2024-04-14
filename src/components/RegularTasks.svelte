<div class="wrapper">
    <div class="wrapper-tag"><span>Regular Tasks</span></div>
    <div class="heading">Regular Tasks</div>
    <ul class="tasks">
        <li class="task">
            <label for="">
                <input type="checkbox" />
                <span>Reading book</span>
            </label>
        </li>
        <li class="task">
            <label for="">
                <input type="checkbox" />
                <span>Work out</span>
            </label>
        </li>
        <li class="task">
            <label for="">
                <input type="checkbox" />
                <span>Reading book</span>
            </label>
        </li>
        <li class="task">
            <label for="">
                <input type="checkbox" />
                <span>Reading book</span>
            </label>
        </li>
        <li class="task">
            <label for="">
                <input type="checkbox" />
                <span>Reading book</span>
            </label>
        </li>
    </ul>
</div>

<style>
    .wrapper {
        position: fixed;
        background-color: var(--paper-color);
        top: 72px;
        left: 100%;
        max-height: 300px;
        width: 300px;
        z-index: 999;
        padding: 16px 16px 8px;
        box-shadow:
            0 10px 15px -3px rgb(0 0 0 / 0.1),
            0 4px 6px -4px rgb(0 0 0 / 0.1);
        transition: all 0.25s ease;
    }

    .wrapper:hover {
        left: calc(100% - 300px);
    }

    .wrapper-tag {
        position: absolute;
        right: 100%;
        top: 0;
        background-color: var(--paper-color);
        height: 55%;
        width: 40px;
        border-radius: 40px 40px 40px 999em;
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: default;
    }

    .wrapper:hover .wrapper-tag span {
        opacity: 0;
    }

    .wrapper-tag span {
        font-size: 14px;
        text-orientation: upright-90deg;
        writing-mode: vertical-rl;
        margin-bottom: 20%;
        font-weight: 600;
        transition: opacity 0.2s ease;
    }

    .heading {
        font-weight: 700;
        font-size: 18px;
        text-align: center;
    }

    .tasks {
        list-style-type: none;
        margin-top: 8px;
    }

    .task {
        display: flex;
        align-items: center;
        padding: 8px 0;
    }

    .task:not(:last-child) {
        border-bottom: 1px solid #ccc;
    }

    .task input {
        margin-right: 8px;
    }

    .task input:checked ~ span {
        text-decoration: line-through;
    }
</style>
