# Mintlify Documentation Templates

## Core Configuration Templates

### Basic docs.json Template
```json
{
  "name": "Your Product Name",
  "logo": {
    "dark": "/logo-dark.svg",
    "light": "/logo-light.svg"
  },
  "favicon": "/favicon.svg",
  "colors": {
    "primary": "#0D9373",
    "light": "#07C983", 
    "dark": "#0D9373"
  },
  "topbarLinks": [
    {
      "name": "Support",
      "url": "mailto:support@yourcompany.com"
    }
  ],
  "topbarCtaButton": {
    "name": "Dashboard",
    "url": "https://dashboard.yourproduct.com"
  },
  "tabs": [
    {
      "name": "API Reference",
      "url": "api-reference"
    },
    {
      "name": "Guides",
      "url": "guides"
    }
  ],
  "anchors": [
    {
      "name": "Community",
      "icon": "github",
      "url": "https://github.com/yourcompany"
    },
    {
      "name": "Blog",
      "icon": "newspaper",
      "url": "https://yourcompany.com/blog"
    }
  ],
  "navigation": [
    {
      "group": "Get Started",
      "pages": [
        "introduction",
        "quickstart", 
        "installation"
      ]
    },
    {
      "group": "Core Concepts",
      "pages": [
        "concepts/overview",
        "concepts/authentication",
        "concepts/configuration"
      ]
    },
    {
      "group": "Guides",
      "pages": [
        "guides/getting-started",
        "guides/advanced-usage",
        "guides/best-practices"
      ]
    },
    {
      "group": "API Reference",
      "pages": [
        "api-reference/introduction",
        "api-reference/authentication",
        "api-reference/endpoints"
      ]
    }
  ],
  "footerSocials": {
    "x": "https://x.com/yourcompany",
    "github": "https://github.com/yourcompany",
    "linkedin": "https://linkedin.com/company/yourcompany"
  },
  "analytics": {
    "gtag": {
      "measurementId": "G-XXXXXXXXXX"
    }
  }
}
```

### Enterprise docs.json Template
```json
{
  "name": "Enterprise Product Suite",
  "logo": {
    "dark": "/logo-dark.svg",
    "light": "/logo-light.svg"
  },
  "favicon": "/favicon.svg",
  "colors": {
    "primary": "#1e40af",
    "light": "#3b82f6",
    "dark": "#1e3a8a"
  },
  "versions": [
    {
      "name": "v2.0",
      "url": "v2"
    },
    {
      "name": "v1.0", 
      "url": "v1"
    }
  ],
  "tabs": [
    {
      "name": "Platform API",
      "url": "platform-api"
    },
    {
      "name": "SDKs",
      "url": "sdks",
      "versions": [
        {
          "version": "latest",
          "anchors": [
            {
              "anchor": "JavaScript",
              "pages": ["sdks/js/installation", "sdks/js/quickstart"]
            },
            {
              "anchor": "Python", 
              "pages": ["sdks/python/installation", "sdks/python/quickstart"]
            }
          ]
        }
      ]
    },
    {
      "name": "Enterprise",
      "url": "enterprise"
    }
  ],
  "auth": {
    "method": "key",
    "name": "X-API-Key"
  },
  "navigation": [
    {
      "group": "Platform Overview",
      "pages": [
        "introduction",
        "architecture",
        "security"
      ]
    },
    {
      "group": "Getting Started",
      "pages": [
        "quickstart",
        "authentication", 
        "first-request"
      ]
    }
  ]
}
```

## Page Templates

### Landing Page Template (introduction.mdx)
```mdx
---
title: "Welcome to [Product Name]"
description: "Comprehensive documentation for [Product Name] - the [brief description of what your product does]"
---

<CardGroup cols={2}>
  <Card title="Quick Start" icon="rocket" href="/quickstart">
    Get up and running in under 5 minutes
  </Card>
  <Card title="API Reference" icon="code" href="/api-reference">
    Complete API documentation and examples
  </Card>
  <Card title="Guides & Tutorials" icon="book-open" href="/guides">
    Step-by-step guides for common use cases
  </Card>
  <Card title="SDKs & Libraries" icon="download" href="/sdks">
    Official SDKs for popular programming languages
  </Card>
</CardGroup>

## What is [Product Name]?

[Product Name] is [detailed description of your product, its purpose, and main benefits]. 

### Key Features

<AccordionGroup>
  <Accordion title="🚀 High Performance">
    [Description of performance capabilities]
  </Accordion>
  <Accordion title="🔒 Enterprise Security">
    [Description of security features]
  </Accordion>
  <Accordion title="📈 Scalable Architecture">
    [Description of scalability features]
  </Accordion>
  <Accordion title="🔧 Developer-Friendly">
    [Description of developer experience features]
  </Accordion>
</AccordionGroup>

## Popular Use Cases

<Tabs>
  <Tab title="E-commerce">
    Perfect for online stores needing [specific functionality]
    
    **Key Benefits:**
    - Feature 1
    - Feature 2  
    - Feature 3
  </Tab>
  <Tab title="Enterprise">
    Ideal for large organizations requiring [specific functionality]
    
    **Key Benefits:**
    - Feature 1
    - Feature 2
    - Feature 3
  </Tab>
  <Tab title="Startups">
    Great for growing companies that need [specific functionality]
    
    **Key Benefits:**
    - Feature 1
    - Feature 2
    - Feature 3
  </Tab>
</Tabs>

## Next Steps

<Steps>
  <Step title="Create Account">
    Sign up for a free account to get started
  </Step>
  <Step title="Get API Keys">
    Generate your API keys from the dashboard
  </Step>
  <Step title="Make Your First Request">
    Follow our quickstart guide to make your first API call
  </Step>
</Steps>

<Note>
Need help getting started? Check out our [comprehensive quickstart guide](/quickstart) or [contact our support team](mailto:support@yourcompany.com).
</Note>
```

### Quickstart Template
```mdx
---
title: "Quickstart Guide"
description: "Get up and running with [Product Name] in under 5 minutes"
---

This quickstart guide will walk you through setting up [Product Name] and making your first successful request.

## Prerequisites

Before you begin, make sure you have:

<Check>
  An active [Product Name] account
</Check>
<Check>
  API keys from your dashboard
</Check>
<Check>
  [Any technical requirements like Node.js, Python, etc.]
</Check>

## Step 1: Installation

<Tabs>
  <Tab title="npm">
    ```bash
    npm install @yourcompany/sdk
    ```
  </Tab>
  <Tab title="yarn">
    ```bash
    yarn add @yourcompany/sdk
    ```
  </Tab>
  <Tab title="pip">
    ```bash
    pip install yourcompany-sdk
    ```
  </Tab>
</Tabs>

## Step 2: Authentication

<CodeGroup>
```javascript JavaScript
const client = new YourCompanySDK({
  apiKey: process.env.YOUR_API_KEY
});
```

```python Python
from yourcompany import Client

client = Client(api_key=os.getenv('YOUR_API_KEY'))
```

```curl cURL
curl -X GET "https://api.yourcompany.com/v1/test" \
  -H "Authorization: Bearer YOUR_API_KEY"
```
</CodeGroup>

<Warning>
Never hardcode your API keys. Use environment variables or a secure configuration management system.
</Warning>

## Step 3: Make Your First Request

<CodeGroup>
```javascript JavaScript
async function example() {
  try {
    const result = await client.getData();
    console.log(result);
  } catch (error) {
    console.error('Error:', error);
  }
}
```

```python Python
try:
    result = client.get_data()
    print(result)
except Exception as error:
    print(f"Error: {error}")
```
</CodeGroup>

## Expected Response

```json
{
  "status": "success",
  "data": {
    "message": "Hello from [Product Name]!",
    "timestamp": "2025-01-15T10:30:00Z"
  }
}
```

## Next Steps

<CardGroup cols={2}>
  <Card title="Explore API Endpoints" href="/api-reference">
    Browse all available API endpoints
  </Card>
  <Card title="View Examples" href="/examples">
    See real-world implementation examples
  </Card>
  <Card title="Read Guides" href="/guides">
    Deep-dive tutorials for advanced features
  </Card>
  <Card title="Join Community" href="https://discord.gg/yourcompany">
    Connect with other developers
  </Card>
</CardGroup>

## Troubleshooting

<AccordionGroup>
  <Accordion title="Authentication Errors">
    **Problem**: Getting 401 Unauthorized errors
    
    **Solution**: 
    - Verify your API key is correct
    - Check that your account is active
    - Ensure you're using the correct base URL
  </Accordion>
  
  <Accordion title="Rate Limiting">
    **Problem**: Getting 429 Too Many Requests errors
    
    **Solution**:
    - Implement exponential backoff
    - Check your rate limits in the dashboard
    - Consider upgrading your plan
  </Accordion>
</AccordionGroup>

<Info>
Still having issues? [Contact our support team](mailto:support@yourcompany.com) for personalized help.
</Info>
```

### API Reference Template
```mdx
---
title: "API Reference"
description: "Complete API documentation for [Product Name]"
---

## Base URL

All API requests should be made to:

```
https://api.yourcompany.com/v1
```

## Authentication

[Product Name] uses API key authentication. Include your API key in the Authorization header:

```bash
Authorization: Bearer YOUR_API_KEY
```

<Warning>
Keep your API keys secure and never share them publicly. Rotate your keys regularly for enhanced security.
</Warning>

## Rate Limiting

API requests are rate limited based on your plan:

| Plan | Requests per minute | Burst limit |
|------|-------------------|-------------|
| Free | 60 | 100 |
| Pro | 1,000 | 2,000 |
| Enterprise | 10,000 | 20,000 |

Rate limit headers are included in all responses:

```
X-RateLimit-Limit: 1000
X-RateLimit-Remaining: 999
X-RateLimit-Reset: 1640995200
```

## Error Handling

All errors return JSON with the following structure:

```json
{
  "error": {
    "code": "INVALID_REQUEST",
    "message": "The request was invalid",
    "details": "Additional error information"
  }
}
```

### Common Error Codes

| Code | Status | Description |
|------|--------|-------------|
| `INVALID_REQUEST` | 400 | The request was malformed |
| `UNAUTHORIZED` | 401 | Invalid or missing API key |
| `FORBIDDEN` | 403 | Insufficient permissions |
| `NOT_FOUND` | 404 | Resource not found |
| `RATE_LIMITED` | 429 | Too many requests |
| `INTERNAL_ERROR` | 500 | Server error |

## Endpoints

<CardGroup cols={2}>
  <Card title="Users" href="/api-reference/users">
    Manage user accounts and profiles
  </Card>
  <Card title="Projects" href="/api-reference/projects">
    Create and manage projects
  </Card>
  <Card title="Analytics" href="/api-reference/analytics">
    Access usage and performance data
  </Card>
  <Card title="Webhooks" href="/api-reference/webhooks">
    Configure event notifications
  </Card>
</CardGroup>
```

### API Endpoint Template
```mdx
---
title: "Get User"
api: "GET https://api.yourcompany.com/v1/users/{id}"
---

Retrieves detailed information about a specific user.

<ParamField path="id" type="string" required>
  The unique identifier for the user
</ParamField>

### Query Parameters

<ParamField query="include" type="string">
  Comma-separated list of related resources to include in the response
  
  **Options**: `profile`, `settings`, `usage`
</ParamField>

<ParamField query="fields" type="string">
  Comma-separated list of fields to include in the response
</ParamField>

### Response

<ResponseField name="id" type="string">
  Unique identifier for the user
</ResponseField>

<ResponseField name="email" type="string">
  User's email address
</ResponseField>

<ResponseField name="name" type="string">
  User's full name
</ResponseField>

<ResponseField name="created_at" type="string">
  ISO 8601 timestamp when the user was created
</ResponseField>

<ResponseField name="profile" type="object">
  User profile information (included when `include=profile`)
  
  <Expandable title="profile">
    <ResponseField name="avatar_url" type="string">
      URL to user's avatar image
    </ResponseField>
    
    <ResponseField name="bio" type="string">
      User's biography
    </ResponseField>
  </Expandable>
</ResponseField>

<RequestExample>
```bash cURL
curl -X GET "https://api.yourcompany.com/v1/users/user_123?include=profile" \
  -H "Authorization: Bearer YOUR_API_KEY"
```

```javascript JavaScript
const user = await client.users.get('user_123', {
  include: ['profile']
});
```

```python Python
user = client.users.get('user_123', include=['profile'])
```
</RequestExample>

<ResponseExample>
```json Success Response
{
  "id": "user_123",
  "email": "john@example.com",
  "name": "John Doe",
  "created_at": "2023-01-15T10:30:00Z",
  "profile": {
    "avatar_url": "https://example.com/avatars/john.jpg",
    "bio": "Software developer passionate about APIs"
  }
}
```

```json Error Response
{
  "error": {
    "code": "NOT_FOUND",
    "message": "User not found",
    "details": "No user exists with ID 'user_123'"
  }
}
```
</ResponseExample>
```

### Tutorial/Guide Template
```mdx
---
title: "Building Your First Integration"
description: "A comprehensive guide to integrating [Product Name] into your application"
---

In this tutorial, you'll learn how to integrate [Product Name] into your application from start to finish. By the end, you'll have a working integration that [describe the end goal].

## What You'll Build

We'll create a [description of the final product], which will:

- ✅ Feature 1
- ✅ Feature 2  
- ✅ Feature 3
- ✅ Feature 4

## Prerequisites

<Steps>
  <Step title="Technical Requirements">
    - [Programming language/framework] (version X.X+)
    - [Database/service] account
    - Basic knowledge of [relevant concepts]
  </Step>
  
  <Step title="Account Setup">
    - Active [Product Name] account
    - API keys configured
    - Development environment ready
  </Step>
</Steps>

## Step 1: Project Setup

Let's start by setting up our project structure:

<Tabs>
  <Tab title="Node.js">
    ```bash
    mkdir my-integration
    cd my-integration
    npm init -y
    npm install @yourcompany/sdk express
    ```
  </Tab>
  
  <Tab title="Python">
    ```bash
    mkdir my-integration
    cd my-integration
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    pip install yourcompany-sdk flask
    ```
  </Tab>
</Tabs>

Create your main application file:

<CodeGroup>
```javascript app.js
const express = require('express');
const { YourCompanySDK } = require('@yourcompany/sdk');

const app = express();
const client = new YourCompanySDK({
  apiKey: process.env.YOUR_API_KEY
});

// We'll add more code here
```

```python app.py
from flask import Flask
from yourcompany import Client

app = Flask(__name__)
client = Client(api_key=os.getenv('YOUR_API_KEY'))

# We'll add more code here
```
</CodeGroup>

## Step 2: Basic Integration

Now let's implement the core functionality:

<CodeGroup>
```javascript JavaScript
app.get('/data', async (req, res) => {
  try {
    const result = await client.fetchData({
      limit: req.query.limit || 10
    });
    
    res.json({
      success: true,
      data: result
    });
  } catch (error) {
    res.status(500).json({
      success: false,
      error: error.message
    });
  }
});
```

```python Python
@app.route('/data')
def get_data():
    try:
        limit = request.args.get('limit', 10, type=int)
        result = client.fetch_data(limit=limit)
        
        return jsonify({
            'success': True,
            'data': result
        })
    except Exception as error:
        return jsonify({
            'success': False,
            'error': str(error)
        }), 500
```
</CodeGroup>

<Note>
This endpoint demonstrates the basic pattern for fetching data. All our subsequent endpoints will follow a similar structure.
</Note>

## Step 3: Advanced Features

Let's add some more sophisticated functionality:

<Accordion title="Real-time Updates">
```javascript
const WebSocket = require('ws');

const wss = new WebSocket.Server({ port: 8080 });

client.on('data-updated', (data) => {
  wss.clients.forEach(client => {
    if (client.readyState === WebSocket.OPEN) {
      client.send(JSON.stringify({
        type: 'update',
        data: data
      }));
    }
  });
});
```
</Accordion>

<Accordion title="Error Handling & Retry Logic">
```javascript
const retry = async (fn, maxRetries = 3) => {
  for (let i = 0; i < maxRetries; i++) {
    try {
      return await fn();
    } catch (error) {
      if (i === maxRetries - 1) throw error;
      await new Promise(resolve => setTimeout(resolve, 1000 * Math.pow(2, i)));
    }
  }
};
```
</Accordion>

## Step 4: Testing Your Integration

Let's verify everything works correctly:

```bash
# Start your application
npm start  # or python app.py

# Test the endpoint
curl http://localhost:3000/data?limit=5
```

Expected response:
```json
{
  "success": true,
  "data": [
    {
      "id": "item_1",
      "name": "Sample Item",
      "created_at": "2023-01-15T10:30:00Z"
    }
  ]
}
```

## Production Considerations

<Warning>
Before deploying to production, make sure to:

- Set up proper environment variables
- Implement rate limiting
- Add comprehensive error logging
- Configure monitoring and alerts
</Warning>

### Environment Variables

Create a `.env` file:
```bash
YOUR_API_KEY=your_actual_api_key
NODE_ENV=production
PORT=3000
```

### Security Best Practices

<CardGroup cols={2}>
  <Card title="API Key Security" icon="shield">
    - Use environment variables
    - Rotate keys regularly
    - Monitor usage patterns
  </Card>
  
  <Card title="Rate Limiting" icon="clock">
    - Implement client-side limits
    - Handle 429 responses gracefully
    - Use exponential backoff
  </Card>
</CardGroup>

## Next Steps

Congratulations! You've successfully built your first integration. Here's what you can explore next:

<Steps>
  <Step title="Add More Features">
    Explore our [Advanced Features Guide](/guides/advanced-features)
  </Step>
  
  <Step title="Optimize Performance">
    Learn about [Performance Best Practices](/guides/performance)
  </Step>
  
  <Step title="Deploy to Production">
    Follow our [Deployment Guide](/guides/deployment)
  </Step>
</Steps>

## Troubleshooting

<AccordionGroup>
  <Accordion title="Common Integration Issues">
    **Connection timeouts**: Increase timeout values and implement retry logic
    
    **Rate limiting**: Implement exponential backoff and respect rate limit headers
    
    **Authentication errors**: Verify API key and check account status
  </Accordion>
  
  <Accordion title="Performance Issues">
    **Slow responses**: Use pagination and implement caching
    
    **Memory leaks**: Properly close connections and clean up resources
    
    **High CPU usage**: Optimize data processing and use async operations
  </Accordion>
</AccordionGroup>

<Info>
Need more help? Join our [developer community](https://discord.gg/yourcompany) or [contact support](mailto:support@yourcompany.com).
</Info>
```

## Specialized Templates

### SDK Documentation Template
```mdx
---
title: "[Language] SDK"
description: "Official [Language] SDK for [Product Name]"
---

## Installation

<Tabs>
  <Tab title="npm">
    ```bash
    npm install @yourcompany/sdk
    ```
  </Tab>
  <Tab title="yarn">
    ```bash
    yarn add @yourcompany/sdk
    ```
  </Tab>
</Tabs>

## Quick Start

```javascript
import { YourCompanySDK } from '@yourcompany/sdk';

const client = new YourCompanySDK({
  apiKey: 'your-api-key'
});

// Example usage
const data = await client.getData();
```

## Configuration Options

<ParamField body="apiKey" type="string" required>
  Your API key from the dashboard
</ParamField>

<ParamField body="baseUrl" type="string" default="https://api.yourcompany.com/v1">
  Base URL for API requests
</ParamField>

<ParamField body="timeout" type="number" default="30000">
  Request timeout in milliseconds
</ParamField>

<ParamField body="retries" type="number" default="3">
  Number of retry attempts for failed requests
</ParamField>

## Methods

### getData()

Fetches data from the API.

```javascript
const data = await client.getData({
  limit: 10,
  offset: 0
});
```

**Parameters:**
- `limit` (number, optional): Number of items to return
- `offset` (number, optional): Number of items to skip

**Returns:** Promise<DataResponse>

### createItem(data)

Creates a new item.

```javascript
const item = await client.createItem({
  name: 'New Item',
  description: 'Item description'
});
```

## Error Handling

The SDK throws typed errors for different scenarios:

```javascript
import { ApiError, ValidationError } from '@yourcompany/sdk';

try {
  const data = await client.getData();
} catch (error) {
  if (error instanceof ApiError) {
    console.log('API Error:', error.message);
  } else if (error instanceof ValidationError) {
    console.log('Validation Error:', error.details);
  }
}
```
```

### Changelog Template
```mdx
---
title: "Changelog"
description: "Track updates and changes to [Product Name]"
---

<Update title="New Feature: Real-time Webhooks" date="2025-01-15">
We've added support for real-time webhooks to keep your applications in sync.

**What's New:**
- Webhook endpoint configuration
- Event filtering and routing
- Automatic retry with exponential backoff
- Comprehensive delivery logs

[Learn more about webhooks →](/webhooks)
</Update>

<Update title="API Rate Limit Improvements" date="2025-01-10">
We've increased rate limits across all plans and improved error messaging.

**Changes:**
- Free plan: 60 → 100 requests/minute
- Pro plan: 1,000 → 2,000 requests/minute  
- Enterprise: Custom limits available

**Migration Guide:**
No action required - these changes are automatically applied to all accounts.
</Update>

<Update title="Breaking Change: Authentication Update" date="2025-01-05" type="breaking">
We're updating our authentication system for enhanced security.

**What's Changing:**
- API keys now require `Bearer` prefix
- Old format will be deprecated on March 1, 2025

**Migration Steps:**
1. Update your Authorization header format
2. Test your integration in staging
3. Deploy the changes to production

```diff
- Authorization: YOUR_API_KEY
+ Authorization: Bearer YOUR_API_KEY
```

[View migration guide →](/migration/auth-update)
</Update>
```

## Component Pattern Library

### Navigation Patterns
```mdx
<!-- Tab-based navigation -->
<Tabs>
  <Tab title="Getting Started">
    Content for beginners
  </Tab>
  <Tab title="Advanced">
    Content for experienced users
  </Tab>
</Tabs>

<!-- Accordion FAQ pattern -->
<AccordionGroup>
  <Accordion title="How do I get started?">
    Follow our quickstart guide...
  </Accordion>
  <Accordion title="What are the rate limits?">
    Rate limits vary by plan...
  </Accordion>
</AccordionGroup>

<!-- Step-by-step process -->
<Steps>
  <Step title="Step 1">
    Do this first thing
  </Step>
  <Step title="Step 2">
    Then do this
  </Step>
</Steps>
```

### Content Organization Patterns
```mdx
<!-- Feature overview cards -->
<CardGroup cols={3}>
  <Card title="Fast" icon="zap">
    High-performance API with 99.9% uptime
  </Card>
  <Card title="Secure" icon="shield">
    Enterprise-grade security and compliance
  </Card>
  <Card title="Scalable" icon="trending-up">
    Scales from startup to enterprise
  </Card>
</CardGroup>

<!-- Information hierarchy -->
<Note>
General information or tips
</Note>

<Info>
Important information to highlight
</Info>

<Warning>
Cautions or potential issues
</Warning>

<Tip>
Helpful suggestions or best practices
</Tip>
```

These templates provide a solid foundation for creating comprehensive, user-friendly documentation with Mintlify. Customize them based on your specific product needs and brand guidelines.