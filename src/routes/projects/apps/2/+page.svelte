<h1>Учет расходов</h1>
<input bind:value={newItem} type="text" placeholder="название">
<br><p><input bind:value={newAmount} type="text" placeholder="сумма"></p>
{#if newItem === ""  && newAmount === ""}
    <button>добавить</button>
{:else}
    <button on:click={addExpense}>добавить</button>
{/if}
<table>
<thead>
    <tr>
        <th>Название</th>
        <th>Сумма</th>
        <th>Действия</th>
    </tr>
</thead>
<tbody>
    {#each expenses as expense, index}
        <tr>
            <td><div>{expense.name}</div></td>
            <td><div>{expense.amount}</div></td>
            <td><button on:click={() => deleteExpense(index)}>delete</button></td>
        </tr>
    {/each}
</tbody>
</table>

<script>
    let expenses = [];
    let newItem = "";
    let newAmount = "";
    function addExpense(){
        const obj = {
            name: newItem,
            amount: parseInt(newAmount)
        };
        expenses.push(obj)
        expenses = expenses;
        newItem = "";
        newAmount = "";
    }
    function deleteExpense(index){
        expenses.splice(index, 1)
        expenses = expenses;
    }
</script>

<style>
    input[type="text"]{
        padding: 5px;
        border: 1px solid #ccc;
        border-radius: 5px;
        margin-right: 10px;
        width: 150px;
    }
    table{
        margin-top: 20px;
        border-collapse: collapse;
        width: 100%;
    }
    th,
    td{
        border: 1px solid #ccc;
        padding: 8px;
        text-align: left;
    }
    th{
        background-color: #eee;
    }
    button{
        padding: 5px 10px;
        background-color: #4caf50;
        color:white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
    }
    h1{
        font-size: 24px;
        margin-bottom: 20px;
    }
</style>