# todo_app
Mahitha Karnati
karnatim

Each todo is automatically assigned a priority level (high, medium, or low) when it is created.  
The priority is inferred using an LLM based on the todo’s title.
Users can:
- Filter todos by priority (All , High , Medium , Low)
- Toggle sorting so higher-priority todos appear first
This makes the todo list more useful for task planning and time management.

Relevant code:
`main.jac`
  - `enum Priority`
  - `def suggest_priority(...)`
  - `node Todo`
  - `AddTodo` and `ListTodos` walkers
- `frontend.cl.jac`
  - State variables: `priorityFilter`, `sortByPriority`
  - UI controls for filtering and sorting
- `frontend.impl.jac`
  - `visibleTodos()` function 
