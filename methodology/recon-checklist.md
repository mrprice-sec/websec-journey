# Web App Recon Checklist

A starting-point checklist for approaching an unfamiliar target
systematically — expand this as you learn what matters for different
app types.

## 1. Map the application
- [ ] Crawl manually (click through as a normal user) while proxying through Burp
- [ ] Note every distinct endpoint, parameter, and cookie
- [ ] Identify authentication/session mechanism
- [ ] Identify roles/permission levels if multi-user

## 2. Understand the tech stack
- [ ] Check response headers (server, framework hints)
- [ ] Check for exposed error messages / stack traces
- [ ] Look for JS files revealing client-side logic or hidden endpoints

## 3. Test access control boundaries
- [ ] Try accessing other users' resources by changing IDs
- [ ] Try accessing higher-privilege functionality as a lower-privilege user
- [ ] Test both horizontal and vertical privilege escalation

## 4. Test input handling
- [ ] Identify every place user input is reflected or stored
- [ ] Test for XSS in each (reflected, stored, DOM)
- [ ] Test for injection in query/form parameters (SQLi, command injection)

## 5. Test trust assumptions
- [ ] Any server-side requests based on user input? (SSRF candidates)
- [ ] Any file uploads? What's validated — extension, content, both?
- [ ] Any deserialization of user-controlled data?

## 6. Business logic
- [ ] Can steps be skipped or reordered (e.g. checkout flow)?
- [ ] Can values be manipulated that shouldn't be client-controlled (price, quantity)?

## 7. Document as you go
- [ ] Screenshot/save requests for anything interesting immediately — don't rely on memory
- [ ] Note dead ends too — they matter for the writeup's methodology section
