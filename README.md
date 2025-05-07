#!/bin/bash

# تحديد المجلدات التي نحتاج لإنشائها
mkdir -p src/components src/pages src/routes src/controllers src/models public

# إنشاء ملفات المشروع الأساسية
touch index.js
touch src/App.jsx
touch src/index.html
touch src/pages/HomePage.jsx
touch src/pages/LoginPage.jsx
touch src/pages/BookingPage.jsx
touch src/routes/routes.js
touch src/controllers/bookingController.js
touch src/controllers/authController.js
touch src/models/userModel.js

# إضافة الأكواد الأساسية للملفات

# index.js
echo "const express = require('express');" > index.js
echo "const app = express();" >> index.js
echo "const port = 3000;" >> index.js
echo "app.listen(port, () => console.log('Server running on port ${port}'));" >> index.js

# src/index.html
echo "<!DOCTYPE html>" > src/index.html
echo "<html lang='en'>" >> src/index.html
echo "<head>" >> src/index.html
echo "  <meta charset='UTF-8'>" >> src/index.html
echo "  <meta name='viewport' content='width=device-width, initial-scale=1.0'>" >> src/index.html
echo "  <title>طويق للنقل البري الدولي</title>" >> src/index.html
echo "</head>" >> src/index.html
echo "<body>" >> src/index.html
echo "  <h1>مرحبا بك في نظام طويق للنقل البري الدولي!</h1>" >> src/index.html
echo "</body>" >> src/index.html
echo "</html>" >> src/index.html

# src/App.jsx
echo "import React from 'react';" > src/App.jsx
echo "import HomePage from './pages/HomePage';" >> src/App.jsx
echo "const App = () => {" >> src/App.jsx
echo "  return (" >> src/App.jsx
echo "    <div>" >> src/App.jsx
echo "      <HomePage />" >> src/App.jsx
echo "    </div>" >> src/App.jsx
echo "  );" >> src/App.jsx
echo "};" >> src/App.jsx
echo "export default App;" >> src/App.jsx

# src/pages/HomePage.jsx
echo "import React from 'react';" > src/pages/HomePage.jsx
echo "const HomePage = () => {" >> src/pages/HomePage.jsx
echo "  return (" >> src/pages/HomePage.jsx
echo "    <div>" >> src/pages/HomePage.jsx
echo "      <h2>الصفحة الرئيسية</h2>" >> src/pages/HomePage.jsx
echo "    </div>" >> src/pages/HomePage.jsx
echo "  );" >> src/pages/HomePage.jsx
echo "};" >> src/pages/HomePage.jsx
echo "export default HomePage;" >> src/pages/HomePage.jsx

# src/pages/LoginPage.jsx
echo "import React from 'react';" > src/pages/LoginPage.jsx
echo "const LoginPage = () => {" >> src/pages/LoginPage.jsx
echo "  return (" >> src/pages/LoginPage.jsx
echo "    <div>" >> src/pages/LoginPage.jsx
echo "      <h2>تسجيل الدخول</h2>" >> src/pages/LoginPage.jsx
echo "    </div>" >> src/pages/LoginPage.jsx
echo "  );" >> src/pages/LoginPage.jsx
echo "};" >> src/pages/LoginPage.jsx
echo "export default LoginPage;" >> src/pages/LoginPage.jsx

# src/pages/BookingPage.jsx
echo "import React from 'react';" > src/pages/BookingPage.jsx
echo "const BookingPage = () => {" >> src/pages/BookingPage.jsx
echo "  return (" >> src/pages/BookingPage.jsx
echo "    <div>" >> src/pages/BookingPage.jsx
echo "      <h2>صفحة الحجز</h2>" >> src/pages/BookingPage.jsx
echo "    </div>" >> src/pages/BookingPage.jsx
echo "  );" >> src/pages/BookingPage.jsx
echo "};" >> src/pages/BookingPage.jsx
echo "export default BookingPage;" >> src/pages/BookingPage.jsx

# src/routes/routes.js
echo "const express = require('express');" > src/routes/routes.js
echo "const router = express.Router();" >> src/routes/routes.js
echo "router.get('/', (req, res) => {" >> src/routes/routes.js
echo "  res.send('مرحبًا بك في نظام طويق للنقل البري الدولي');" >> src/routes/routes.js
echo "});" >> src/routes/routes.js
echo "module.exports = router;" >> src/routes/routes.js

# src/controllers/bookingController.js
echo "const bookingController = {};" > src/controllers/bookingController.js
echo "module.exports = bookingController;" >> src/controllers/bookingController.js

# src/controllers/authController.js
echo "const authController = {};" > src/controllers/authController.js
echo "module.exports = authController;" >> src/controllers/authController.js

# src/models/userModel.js
echo "const userModel = {};" > src/models/userModel.js
echo "module.exports = userModel;" >> src/models/userModel.js

# تأكيد بنجاح إنشاء الملفات
echo "تم إنشاء جميع الملفات والمجلدات بنجاح!"
