# Copilot Instructions

## Required Checklist
Before completing code changes, run from the repository root:
- [ ] Lint: `dotnet format SocOps/SocOps.csproj --verify-no-changes`
- [ ] Build: `dotnet build SocOps/SocOps.csproj`
- [ ] Test: `dotnet test`; report if no tests are available.

## Project
Soc Ops is a .NET 10 Blazor WebAssembly Social Bingo game, not an ASP.NET Core Web API.

## Guidance
- Keep routes, UI, game state/rules, models, and prompts in their respective `SocOps/Pages/`, `Components/`, `Services/`, `Models/`, and `Data/` folders.
- Preserve `BingoGameService` state notifications and versioned local-storage persistence.
- Follow existing C# nullable/implicit-using settings and the scoped CSS/frontend instructions; keep translated workshop guides aligned.
- Run locally with `dotnet run --project SocOps/SocOps.csproj`. Avoid generated `bin/`, `obj/`, and `.solutions/` snapshots unless requested.
