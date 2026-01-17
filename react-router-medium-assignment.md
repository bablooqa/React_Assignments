# React Router Medium-Level Assignment (20 Questions)

## Instructions
- Create separate components for each scenario.
- Use `BrowserRouter`, `Routes`, `Route`, `Link`, `useNavigate`, and `useParams`.
- Follow component-based architecture.
- Use functional components only.

---

## Section A: Component-Based Routing (1–8)

1. Create a `Home` component and set it as the default route (`/`).

2. Create an `About` component and configure routing so it loads at `/about`.

3. Create a `Navbar` component with `Link` for:
   - Home
   - About
   - Contact

4. Create a `Contact` component and route it using React Router.

5. Create a `Layout` component that contains a navbar and an `<Outlet />` for child routes.

6. Implement nested routing for:
   - `/dashboard`
   - `/dashboard/profile`
   - `/dashboard/settings`

7. Create separate components for `Profile` and `Settings` under `Dashboard`.

8. Add a wildcard route to display a `PageNotFound` component.

---

## Section B: Scenario-Based Navigation (9–14)

9. Create a `Login` component with a button that navigates to `/dashboard` using `useNavigate`.

10. After successful login, redirect the user automatically to the Dashboard page.

11. Create a `Logout` button that navigates the user back to the Home page.

12. Disable direct access to `/dashboard` unless the user is logged in (basic logic only).

13. Create a button in the Dashboard that navigates back to the previous page.

14. Navigate to a route after submitting a form using `useNavigate`.

---

## Section C: Dynamic Routing with useParams (15–20)

15. Create a `Products` component that displays a list of products.

16. When clicking a product, navigate to `/product/:id`.

17. Create a `ProductDetails` component and fetch the product ID using `useParams`.

18. Display product details based on the dynamic `id`.

19. Handle an invalid product ID gracefully.

20. Add a `Back to Products` button using `useNavigate`.

---

## Bonus Challenge (Optional)

- Create a `ProtectedRoute` component.
- Redirect unauthenticated users to `/login`.
- Maintain login state using `useState`.

---

## Folder Structure Suggestion
src/
│── components/
│ ├── Navbar.jsx
│ ├── Layout.jsx
│
│── pages/
│ ├── Home.jsx
│ ├── About.jsx
│ ├── Contact.jsx
│ ├── Login.jsx
│ ├── Dashboard.jsx
│ ├── Profile.jsx
│ ├── Settings.jsx
│ ├── Products.jsx
│ ├── ProductDetails.jsx
│ ├── PageNotFound.jsx
│
│── App.jsx
│── main.jsx


---

## Evaluation Criteria
- Proper routing setup
- Clean component structure
- Correct usage of hooks
- Navigation works as expected
- Code readability



