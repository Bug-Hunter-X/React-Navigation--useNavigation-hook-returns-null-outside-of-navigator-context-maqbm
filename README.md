# React Navigation useNavigation Hook Error

This repository demonstrates a common error encountered when using React Navigation's `useNavigation` hook: it returns null when used outside of the navigator's context. This can lead to unexpected behavior and runtime errors.

**Problem:** The `useNavigation` hook within `MyComponent` attempts to use navigation methods while outside the scope of a `NavigationContainer` or other navigation component.

**Solution:** Ensure that `MyComponent` is rendered within the tree of a `NavigationContainer` (or other relevant navigation structure).   If it's nested deeply, check the parent components to confirm the appropriate navigation context is properly passed down.