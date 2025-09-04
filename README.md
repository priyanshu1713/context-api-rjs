# React User Context Example

A simple demo of React Context API with a custom provider.  
- `UserContext.js` → defines the context.  
- `UserContextProvider.jsx` → manages state (`user`, `setUser`) and provides it.  
- Components (e.g., Navbar, Profile) → use `useContext(UserContext)` to access/update shared data.  

**Example:** Click "Login" in Profile → Navbar instantly shows "Hi, Priyanshu".  

Run locally:  
```bash
npm install
npm start
