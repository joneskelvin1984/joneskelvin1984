# AWS Account Configuration, Budget & Alarm Setup

## Project Overview
This project demonstrates the essential first steps in AWS account management, focusing on security best practices and cost control. I've configured IAM access, billing alerts, and budget monitoring to establish a solid foundation for AWS cloud operations.

## Technologies Used
- AWS Identity and Access Management (IAM)
- AWS Budgets
- AWS Cost Explorer
- CloudWatch Billing Alerts
- AWS Free Tier Monitoring

## Implementation Steps

### Setting an IAM Account Alias
1. Logged in to AWS using root user credentials
2. Navigated to the IAM dashboard through the search bar
3. Located the "AWS Account" section in the IAM dashboard
4. Created a unique account alias for simplified login access
5. Documented the new sign-in URL for IAM user access

### Enabling IAM User Access to Billing
1. Accessed Account settings through the account name dropdown
2. Located "IAM user and role access to Billing information" section
3. Activated billing access for IAM users and roles
4. Verified the settings were successfully updated
5. Documented the change for security documentation

### Updating Billing Preferences
1. Configured Alert preferences:
   - Enabled AWS Free Tier usage alerts
   - Activated CloudWatch billing alerts
   - Set up email notifications for billing alerts
2. Customized Delivery preferences:
   - Configured invoice delivery via PDF email
   - Ensured all essential billing communications are received

### Creating a Budget with Alerts
1. Created a monthly cost budget using AWS Budgets
2. Set a conservative budget threshold of $5 to ensure tight cost control
3. Configured alert thresholds at 85% and 100% of the budget
4. Added email notification destinations
5. Verified budget creation and alert settings

## Challenges and Solutions

### Challenge: Understanding IAM Best Practices
**Issue:** Determining the optimal IAM configuration for a secure yet functional account setup.  
**Solution:** Researched AWS security best practices and implemented principle of least privilege by enabling only necessary billing access for IAM users.

### Challenge: Budget Alert Configuration
**Issue:** Deciding on appropriate budget thresholds and notification settings.  
**Solution:** Set conservative budget limits with early warning thresholds (85%) to ensure ample time to respond to potential cost overruns before reaching the budget limit.

## Screenshots/Steps

Step 1: IAM Account Alias Setup
The IAM account alias creates a custom URL for accessing your AWS account, making it easier to remember and more secure than using the account ID.

### IAM Dashboard Configuration
![Screenshot 2025-05-02 at 11 24 30 AM](https://github.com/user-attachments/assets/3461e58e-11d5-4342-abe3-d06e4a9fe5e5)
![Screenshot 2025-05-02 at 11 25 42 AM](https://github.com/user-attachments/assets/38c63bed-6dc6-40ea-884c-a7a69b215b03)
![Screenshot 2025-05-02 at 11 26 02 AM](https://github.com/user-attachments/assets/50d837d8-4e18-4a9f-82e1-bac46fbaa60d)
![Screenshot 2025-05-02 at 11 26 26 AM](https://github.com/user-attachments/assets/8320ffa9-8d87-432a-a668-64985cc6af07)

Step 2: Billing Access Configuration
Enabling IAM access to billing is critical for delegating financial monitoring without sharing root credentials.
### Billing Access Settings
![Screenshot 2025-05-02 at 11 28 19 AM](https://github.com/user-attachments/assets/9606318d-5a93-4b44-8f62-bacdab73ea85)
![Screenshot 2025-05-02 at 11 28 28 AM](https://github.com/user-attachments/assets/278d15cb-c2c7-4f71-9faa-afa57cd1f485)
![Screenshot 2025-05-02 at 11 28 40 AM](https://github.com/user-attachments/assets/e3c3eca9-7595-4724-a7db-350fc40064c3)
![Screenshot 2025-05-02 at 11 29 10 AM](https://github.com/user-attachments/assets/e2522201-ee5a-48e0-ba75-2cb0400a5f18)


Step 3: Budget Creation Process
AWS Budgets provides proactive monitoring of AWS costs and usage. The monthly budget template offers the following advantages:

-Consistent monthly tracking aligned with billing cycles
-Customizable alert thresholds
-Multiple notification recipients
-Integration with AWS Cost Explorer for detailed analysis

### Budget Alert Configuration
![Screenshot 2025-05-02 at 11 29 25 AM](https://github.com/user-attachments/assets/5dd88080-f25a-49e9-b4d9-21f2ea975d8f)
![Screenshot 2025-05-02 at 11 30 03 AM](https://github.com/user-attachments/assets/ad240aee-1ab1-4e62-86ef-3e6b7a9fcf21)
![Screenshot 2025-05-02 at 11 30 13 AM](https://github.com/user-attachments/assets/14d2745b-7ed4-44f5-8531-954937e9da8d)


Step 4: Monitoring and Maintenance
After setup, regularly:

-Review Cost Explorer data to identify usage patterns
-Adjust budget thresholds as needed based on actual usage
-Verify alert emails are being received and not filtered as spam
-Consider setting up additional budgets for specific services as your AWS usage expands

### Cost Explorer View
![Screenshot 2025-05-02 at 11 31 08 AM](https://github.com/user-attachments/assets/4d87fa35-23a6-4ebf-85c6-8ace185b5694)
![Screenshot 2025-05-02 at 11 31 20 AM](https://github.com/user-attachments/assets/65ca2419-46ed-4add-9aaf-b9dd683d192c)
![Screenshot 2025-05-02 at 11 31 27 AM](https://github.com/user-attachments/assets/896010d2-66bf-4390-a287-60f45074586e)
![Screenshot 2025-05-02 at 11 33 17 AM](https://github.com/user-attachments/assets/cfc4de47-517c-4b60-94d9-48b86fc79e11)
![Screenshot 2025-05-02 at 11 34 02 AM](https://github.com/user-attachments/assets/403d0c3b-850a-4b52-87ab-e6d775c12e69)


## Documentation

Best Practices Implemented

Early Warning System: Set alerts below the full budget amount to enable proactive response
Documentation: Maintained records of all configuration changes
Principle of Least Privilege: Limited billing access to only necessary IAM roles
Regular Monitoring: Established routine for reviewing cost data

Future Improvements

Implement AWS Organizations for more granular budget control across multiple accounts
Create service-specific budgets as usage patterns become more defined
Set up AWS Cost Anomaly Detection to identify unusual spending patterns
Develop automated responses to budget alerts using AWS Lambda

References

AWS IAM Best Practices
AWS Budgets Documentation
AWS Cost Explorer Guide
