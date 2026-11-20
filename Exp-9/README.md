# Experiment 9: Password-Guessing Risks and Defenses

## Aim

To understand how repeated password attempts can threaten authentication and to identify controls that help detect and prevent password guessing.

## Requirements and scope

- An instructor-provided, isolated lab or a supplied sample authentication log
- A test account with dummy credentials, if a hands-on demonstration is part of the course
- No production accounts, real user credentials, or systems outside the explicitly authorized lab

This write-up focuses on the security impact and defensive review. Do not direct password-guessing tools at public services or accounts. Keep any instructor-approved test restricted to the designated lab target and stop if it reaches any other system.

## Theory

Password-guessing attacks try candidate passwords against an authentication mechanism. Repeated failures can indicate guessing activity, while weak or reused passwords can make an account more vulnerable. Defenses include unique passwords stored with a password manager, multi-factor authentication, rate limiting, progressive delays, account lockout policies designed to avoid denial of service, and monitoring for unusual authentication failures.

Hydra is an authentication-testing tool. Its use is appropriate only in a controlled environment with explicit authorization; this experiment does not provide commands, wordlists, or target-selection instructions.

## Procedure

1. Confirm the exercise scope with the instructor. Record the approved lab boundary and the dummy account or sample log being used.
2. Review the authentication policy and identify protections such as rate limits, multi-factor authentication, and alerting.
3. Use only the instructor-provided demonstration or sample authentication events. Do not test real accounts or reuse real passwords.
4. Review the resulting events for repeated failures, lockout behavior, and whether the configured defenses generated an alert.
5. Record the observations without including passwords, tokens, or personally identifying information.

## Result

Document whether repeated failed attempts were visible in the supplied lab evidence and which protective controls responded. If no alert or rate limit was observed, report that as a defensive improvement rather than attempting tests against another system.

## Conclusion

Password guessing is a risk to weakly protected authentication services. Strong unique passwords, multi-factor authentication, sensible throttling, and timely monitoring reduce that risk. Testing must remain within the expressly authorized lab scope.
