# React User Context Example

This project demonstrates how to use **React Context API** with a custom provider to share state across multiple components without prop drilling.

## Files

- **UserContext.js**  
  Creates the context object using `createContext()`.

- **UserContextProvider.jsx**  
  A provider component that holds the `user` state and exposes it (along with `setUser`) to all children using `UserContext.Provider`.

- **Example Components (Navbar, Profile, etc.)**  
  Show how different components can access and update the same shared `user` data using `useContext(UserContext)`.

## How it Works

1. `UserContext.js` → defines the context (like an empty container).  
2. `UserContextProvider.jsx` → manages the `user` state and provides it to all child components.  
3. Child components (e.g., `Navbar`, `Profile`) → use `useContext(UserContext)` to read and update the `user`.  
4. When `setUser` is called, React re-renders the provider and all subscribed components automatically update.

## Example Flow

- Initially, `user` is `null`.  
- A component (like `Profile`) can call `setUser("Priyanshu")`.  
- Now all components inside `UserContextProvider` instantly see `user = "Priyanshu"`.

---

### Run Locally

```bash
npm install
npm start
