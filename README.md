# OE: Deployment project

### Problem Statement
Local installment shop owners face significant challenges in managing their businesses efficiently due to reliance on outdated paper-based systems. These systems result in manual and time-consuming processes for tracking customer payments, managing product inventory, and maintaining records. As a result, installment shop owners often struggle with operational inefficiencies, inventory discrepancies, and poor customer service. There is a pressing need for a digital solution that streamlines operations, improves inventory management, enhances customer communication, and ensures a seamless installment-based purchasing experience for both shop owners and customers

### Background Study:

1.Local Installment Business Model:

- Local installment businesses provide essential goods and services through manageable installment payments.
- These businesses offer financial flexibility to customers who may struggle with large upfront payments.<br>

2.Current Practices:

- Installment shop owners often rely on manual, paper-based systems for managing customer payments and product inventory.
- Communication with customers is primarily in person or via phone calls.
- Inventory management is done manually, leading to inefficiencies and errors.<br>

3.Existing Technologies:

- Generic point-of-sale (POS) systems and inventory management software may not fully meet the needs of installment shop owners.
- Custom software solutions can be costly and may not be accessible to small businesses.
- Limited internet connectivity and technological literacy may hinder adoption of digital solutions in some communities.

### Our Solution

Our project aims to address the challenges faced by installment shop owners by providing a comprehensive digital solution. Our platform will offer features tailored to the specific needs of installment-based businesses, including:

1. Streamlined Operations: Digitizing processes such as customer management, payment tracking, and inventory management to improve efficiency and accuracy.
2. Flexible Payment Options: Offering customizable installment plans and payment schedules to cater to the diverse financial needs of customers.
3. Enhanced Communication: Facilitating seamless communication between shop owners and customers through in-app messaging and notifications.
4. Comprehensive Reporting: Providing detailed insights and analytics to help shop owners make informed business decisions and optimize their operations.
5. User-Friendly Interface: Designing an intuitive and easy-to-navigate interface for both shop owners and customers to ensure a positive user experience.

By leveraging technology to streamline operations and enhance customer service, InstaEase aims to empower installment shop owners to grow their businesses and provide better services to their communities.. 


### How It Works

1. **User Submission:** Users submit their GitHub repository URLs for React projects along with the desired domain via the provided interface.
2. **API Server:** Upon submission, the system hits the API server with the provided information.
3. **Docker Container:** The API server spins up a Docker container from the image already uploaded to Azure Container Repository.
4. **Cloning Repository:** The Docker container clones the specified GitHub repository.
5. **Building:** The Docker container performs npm install and npm run build to generate the build files.
6. **Storage:** Finally, the built files are pushed to a storage bucket in Azure.
7. **Reverse proxy server:** Now when the user will hit the server with "subdomain.deployfor.me", then the reverse proxy server will serve the respective build/static files from the storage bucket.
8. **Automated Testing:** Selenium is employed for automated testing. It will deploy boilerplate and React projects to verify functionality.
9. **Continuous Integration/Deployment (CI/CD):** GitHub Actions are utilized for CI/CD. Upon each commit or push to the API, server test server, and the React front-end, a rebuild is triggered followed by automated testing to ensure project stability and functionality.
10. **DB Integration:** MongoDB for user authentication and data persistence, providing a secure and reliable storage solution for user-related information.


### Architecture
[eraser.io link](https://app.eraser.io/workspace/5BOuL68hzj3ssSMm2WHm?origin=share)

### Design
[Figma link](https://www.figma.com/file/U5ASL9F0MakVyns28J5y5r/OE-Project)
