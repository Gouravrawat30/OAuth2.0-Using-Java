# OAuth2.0 Email Sender in Java

This project demonstrates how to implement OAuth2.0 authorization with Java to send emails using the Gmail API. The project includes a sample program that authenticates with Google, obtains authorization, and sends an email through the authenticated user's Gmail account.

## Project Overview

The project provides:
1. **OAuth2.0 Authentication** - Implements Google’s OAuth2.0 to securely access Gmail.
2. **Email Sending** - Sends an email through the Gmail API, using `javax.mail` and Google’s Java client libraries.

## Prerequisites

Before starting, ensure you have the following:

- **Java Development Kit (JDK)**: Version 8 or later.
- **Google API Client Libraries**: Installed for Java, including Gmail API, OAuth2, and JSON handling.
- **Gmail API Credentials**: Downloaded `credentials.json` file from Google Cloud Console after enabling Gmail API.

## Project Structure

- **emailusingjkarta.java** - Main class that manages OAuth2.0 authorization and sends emails.
- **Dependencies** - Uses the following libraries:
  - Google API Client Libraries (Gmail, OAuth2, JSON)
  - Javax Mail (Jakarta Mail)

## Setup Instructions

### Step 1: Google Cloud Setup

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Enable the **Gmail API** for your project.
3. Configure the **OAuth Consent Screen**.
4. Download the `credentials.json` file and save it to the root directory of the project.

### Step 2: Install Dependencies

Ensure the following dependencies are added in your project:
- Google API Client for OAuth2
- Gmail API Client
- Javax Mail (Jakarta Mail)

Add these to your `pom.xml` if you're using Maven:

```xml
<dependencies>
    <!-- Google API Client -->
    <dependency>
        <groupId>com.google.api-client</groupId>
        <artifactId>google-api-client</artifactId>
        <version>1.32.1</version>
    </dependency>
    <!-- Gmail API -->
    <dependency>
        <groupId>com.google.apis</groupId>
        <artifactId>google-api-services-gmail</artifactId>
        <version>v1-rev110-1.25.0</version>
    </dependency>
    <!-- Jakarta Mail API -->
    <dependency>
        <groupId>com.sun.mail</groupId>
        <artifactId>jakarta.mail</artifactId>
        <version>1.6.7</version>
    </dependency>
</dependencies>
