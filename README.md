# todo-list
T0d0.jsx:
.todo.css {
    width: 600px;
    min-height: 732px;
    border-radius: 20px;
    background: #fff;
    margin: auto;
    margin-top: 174px;
    display: flex;
    flex-direction: column;
    padding: 0px 44px;
    padding-bottom: 30px;
    margin-bottom: 100px;
}

.todo-header {
    margin-top: 84px;
    color: #002765;
    font-size: 36px;
    font-weight: 600;
    line-height: 34px;
}

.todo-add {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 45px;
}

.todo-input {
    border-radius: 50px;
    background: #edeef0;
    border: none;
    width: 578px;
    height: 80px;
    padding-left: 35px;
    font-size: 20px;
}

.todo-add-btn {
    border-radius: 50px;
    background: #ff6739;
    width: 187px;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: -100px;
    color: #fff;
    font-size: 26px;
    font-weight: 600;
    cursor: pointer;
}
Todo.jsx:
import { useRef, useState } from 'react'
import './CSS/Todo.css'

const Todo = () => {

    const [todos,setTodos] = useState([]);
    const inputRef = useRef(null);

    const add = () =>{}
  return (
    <div className='todo'>
        <div className="todo-header">To-Do List</div>
        <div className="todo-add">
            <input ref={inputRef} type="text" placeholder='Add Your Task' className='todo-input'/>
            <div className="todo-add-btn">ADD</div>
        </div>
        <div className="todo-list"></div>
    </div>
  )
}

export default Todo
