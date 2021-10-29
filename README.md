# BlazorHotReloadIssue

Sample Repo to reproduce slow behavior in VS2022 vs dotnet watch


## Steps to reproduce
1. Open project with VS2022 - with enabled hot reload
2. Start project with launch profile "BlazorApp4"
3. Edit index.razor (change/add text or anything else)
4. Press Hot-Reload-Button in Navbar
5. See changes in Browser after 50 to 160 seconds
7. Repeat 3. - 4.  to see subsequent change timings (50 to 160 seconds)

8. Stop project
9. Start with launch profile "With dotnet watch" or simply start project with "dotnet watch run"
10. Edit index.razor (change/add text or anything else)
11. Save File to trigger dotnet watch 
12. See changes in Browser after 10 to 20 seconds
13. Repeat 10. - 11. to see subsequent change timings (~1 second)
