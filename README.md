* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(135deg, rgb(245,178,60),  rgb(197,17,71), rgb(208,10,136), rgb(112,10,208), rgb(75,17,190));
  color: #f0f0f0;
  padding: 20px;
  min-height: 100vh;
}

.container {
  max-width: 900px;
  margin: auto;
}

header {
  text-align: center;
  margin-bottom: 20px;
}

header h1 {
  margin-bottom: 10px;
  font-size: 2em;
  color: #61dafb;
}

header input {
  width: 100%;
  padding: 10px;
  background-color: #2d2d2d;
  border: 1px solid #444;
  color: #f0f0f0;
  border-radius: 5px;
}

form {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
  flex-wrap: wrap;
}

form input,
form select,
form button {
  padding: 10px;
  border-radius: 5px;
  border: none;
}

form input,
form select {
  background-color: #2d2d2d;
  color: #fff;
  border: 1px solid #444;
  flex: 1;
  min-width: 120px;
}

form button {
  background-color: #61dafb;
  color: #1e1e1e;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

form button:hover {
  background-color: #21a1f1;
}

.task-block {
  margin-bottom: 20px;
  padding: 15px;
  border-radius: 8px;
  background: linear-gradient(135deg, rgb(101,101,101), rgb(61,60,60), rgb(28,28,28));
  transition: all 0.3s ease;
}

.task-block h2 {
  margin-bottom: 10px;
  color: #fff;
  font-size: 1.3em;
}

.task-list {
  list-style: none;
  margin-bottom: 10px;
  max-height: 1000px;
  overflow: hidden;
  transition: max-height 0.3s ease;
}

.task-list.collapsed {
  max-height: 60px;
  overflow: hidden;
}

.task-list li {
  background-color: #333;
  padding: 10px;
  margin-bottom: 5px;
  border-radius: 5px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  transition: all 0.3s ease;
}

.task-list li.fade-out {
  opacity: 0;
  transform: scale(0.9);
  transition: opacity 0.4s, transform 0.4s;
}

.task-list li input[type="checkbox"] {
  margin-right: 10px;
}

.toggle-btn {
  background-color: transparent;
  border: 1px solid #555;
  color: #ccc;
  padding: 5px 10px;
  border-radius: 4px;
  cursor: pointer;
  font-size: 0.9em;
}

.toggle-btn:hover {
  background-color: #444;
}

#faible {
  border-left: 5px solid #6fcf97;
}

#moyenne {
  border-left: 5px solid #f2c94c;
}

#élevée {
  border-left: 5px solid #eb5757;
}

.archive {
  background: linear-gradient(135deg, rgb(101,101,101), rgb(61,60,60), rgb(28,28,28));
  border-left: 5px solid ;
  margin-bottom: 60px;
}

.actions-bar {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background: #121212;
  padding: 10px;
  text-align: center;
  display: flex;
  justify-content: space-around;
  z-index: 100;
  border-top: 1px solid #333;
}

.actions-bar button {
  background-color: rgba(62,108,231,0.838);
  color: #f0f0f0;
  border: 1px solid rgb(150,147,157);
  border-radius: 6px;
  padding: 8px 14px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.actions-bar button:hover {
  background-color: #555;
}
.task-item.done .name {
  text-decoration: line-through;
  color: #888;
  opacity: 0.6;
}# To_do_list_by_Faucheur