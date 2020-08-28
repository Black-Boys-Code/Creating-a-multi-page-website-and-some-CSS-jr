<!-- Each line is a file pattern followed by one or more owners.

These owners will be the default owners for everything in the repo. Unless a later match takes precedence, @global-owner1 and @global-owner2 will be requested for review when someone opens a pull request.-->
*.*          @blackboyscode

<!-- Order is important; the last matching pattern takes the most precedence. When someone opens a pull request that only modifies JS files, only @js-owner and not the global owner(s) will be requested for a review.-->
*.js         @blackboyscode

<!-- You can also use email addresses if you prefer. They'll be used to look up users just like we do for commit author emails.-->
*.html         @blackboyscode.com

<!-- In this example, @blackboyscode owns any files in the build/logs directory at the root of the repository and any of its subdirectories. -->
/build/logs/ @blackboyscode

<!-- The `docs/*` pattern will match files like `docs/getting-started.md` but not further nested files like `docs/build-app/troubleshooting.md`. -->
docs/*       @blackboyscode.com

<!-- In this example, @blackboyscode owns any file in an apps directory anywhere in your repository. -->
apps/        @blackboyscode

<!-- In this example, @blackboyscode owns any file in the `/docs` directory in the root of your repository. -->
/docs/       @blackboyscode