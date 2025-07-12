<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>To Do List-ku</title>
  <style>
    body {
      font-family: 'Gill Sans', 'Gill Sans MT', 'Trebuchet MS', sans-serif;
      background-color: #F4E4C9;
      padding: 20px;
    }

    h1 {
      text-align: center;
      line-height: 50px;
      color: #482E1D;
    }

    .input-name {
      text-align: center;
      margin-bottom: 20px;
    }

    .todo-form {
      display: flex;
      gap: 10px;
      margin-bottom: 20px;
      flex-wrap: wrap;
    }

    .todo-form input[type="text"], .todo-form input[type="date"] {
      flex: 1;
      padding: 10px;
      font-size: 16px;
    }

    .todo-form button {
      background-color: #412f26;
      color: #CBB89D;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
    }

    .filter-buttons {
      margin-bottom: 15px;
      text-align: center;
    }

    .filter-buttons button {
      background-color: #412f26;
      color: #CBB89D;
      padding: 8px 16px;
      margin: 0 5px;
      border: none;
      cursor: pointer;
    }

    ul {
      list-style-type: none;
      padding: 0;
      background-color: #CFBB99;
      border-radius: 5px;
      padding: 10px;
      min-height: 50px;
    }

    li {
      padding: 10px;
      margin-bottom: 10px;
      background: #E1D9C9;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-radius: 5px;
    }

    .task-left {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .delete-btn {
      background-color: #5d2510;
      color: rgb(221, 27, 27);
      padding: 5px 10px;
      cursor: pointer;
    }

    .completed {
      text-decoration: line-through;
      opacity: 0.6;
    }

    .no-task {
      text-align: center;
      font-style: italic;
      font-size : 20px;
      color: #BB9F88;
    }
  </style>
</head>
<body>

  <div class="input-name" id="nameSection">
    <h1 style="color: #482E1D;">Welcome!</h1>
    <p style="color: #482E1D;">Can I get your name?</p>
    <input type="text" id="nameInput" placeholder="Type your name~" width="180px">
    <button onclick="setName()">Start</button>
  </div>

  <h1 id="headerTitle" style="display:none;"></h1>

  <div class="todo-form" style="display:none;" id="formSection">
    <input type="text" id="taskInput" placeholder="Write it down...">
    <input type="date" id="dateInput">
    <button onclick="addTask()">Add Task!</button>
  </div>

  <div class="filter-buttons" id="filterSection" style="display:none;">
    <button onclick="filterTasks('all')">All</button>
    <button onclick="filterTasks('active')">Ongoing</button>
    <button onclick="filterTasks('completed')">Completed</button>
  </div>

  <ul id="taskList" style="display:none;"></ul>
  <p class="no-task" id="noTaskText" style="display:none;">Oops, no task yet!</p>

  <script>
    let currentFilter = 'all';

    function setName() {
      const name = document.getElementById('nameInput').value.trim();
      if (name === '') return;

      document.getElementById('headerTitle').textContent = `Hai ${name}! Here's your to do list ⸜(｡˃ w ˂ )⸝♡`; style="color: #482E1D;";
      document.getElementById('headerTitle').style.display = 'block';
      document.getElementById('formSection').style.display = 'flex';
      document.getElementById('filterSection').style.display = 'block';
      document.getElementById('taskList').style.display = 'block';
      document.getElementById('nameSection').style.display = 'none';

      updateTaskMessage();
    }

    function addTask() {
      const taskInput = document.getElementById('taskInput');
      const dateInput = document.getElementById('dateInput');
      const taskList = document.getElementById('taskList');

      const taskText = taskInput.value.trim();
      const taskDate = dateInput.value;

      if (taskText === '') return;

      const li = document.createElement('li');
      li.dataset.completed = 'false';
      li.innerHTML = `
        <div class="task-left">
          <input type="checkbox" onchange="toggleComplete(this)">
          <span>${taskText} <small>(${taskDate})</small></span>
        </div>
        <button class="delete-btn" onclick="deleteTask(this)">Delete</button>
      `;
      taskList.appendChild(li);

      taskInput.value = '';
      dateInput.value = '';

      updateTaskMessage();
    }

    function deleteTask(button) {
      const li = button.parentElement;
      li.remove();
      updateTaskMessage();
    }

    function toggleComplete(checkbox) {
      const li = checkbox.closest('li');
      const span = li.querySelector('span');
      if (checkbox.checked) {
        li.dataset.completed = 'true';
        span.classList.add('completed');
      } else {
        li.dataset.completed = 'false';
        span.classList.remove('completed');
      }
      applyFilter();
    }

    function filterTasks(filterType) {
      currentFilter = filterType;
      applyFilter();
    }

    function applyFilter() {
      const tasks = document.getElementById('taskList').getElementsByTagName('li');
      let visibleCount = 0;

      for (let task of tasks) {
        const isCompleted = task.dataset.completed === 'true';

        if (currentFilter === 'all') {
          task.style.display = '';
          visibleCount++;
        } else if (currentFilter === 'active' && isCompleted) {
          task.style.display = 'none';
        } else if (currentFilter === 'completed' && !isCompleted) {
          task.style.display = 'none';
        } else {
          task.style.display = '';
          visibleCount++;
        }
      }

      document.getElementById('noTaskText').style.display = visibleCount === 0 ? 'block' : 'none';
    }

    function updateTaskMessage() {
      const taskList = document.getElementById('taskList');
      const noTaskText = document.getElementById('noTaskText');
      const inputSectionVisible = document.getElementById('formSection').style.display !== 'none';
      noTaskText.style.display = inputSectionVisible && taskList.children.length === 0 ? 'block' : 'none';
    }
  </script>
</body>
</html>
