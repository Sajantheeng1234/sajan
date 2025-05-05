* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  margin: 0;
  font-family: Arial, sans-serif;
}
/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  padding: 10px 20px;
  color: white;
}

.navbar .logo {
  font-size: 24px;
  color: #007bff;
  font-weight: bold;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 20px;
}

.nav-links li a {
  text-decoration: none;
  color: white;
  transition: color 0.3s;
}

.nav-links li a:hover {
  color: #007bff;
}

/* Hamburger styles */
.hamburger {
  display: none;
  flex-direction: column;
  cursor: pointer;
  gap: 5px;
}

.hamburger span {
  width: 25px;
  height: 3px;
  background: white;
  transition: 0.3s;
}

/* Responsive */
@media (max-width: 768px) {
  .hamburger {
    display: flex;
  }

  .nav-links {
    display: none;
    flex-direction: column;
    background-color: #444;
    position: absolute;
    top: 60px;
    right: 0;
    width: 200px;
    padding: 10px;
  }

  .nav-links.active {
    display: flex;
  }
}
  .nav-links a:hover {
    color: #007bff;
  }
.navbar a::after{
    content: '';
    display: block;
    width: 0;
    height: 2px;
    background-color: rgb(255, 178, 34);
    margin-top: 5px;
}
.navbar a:hover::after{
    width: 100%;
}
