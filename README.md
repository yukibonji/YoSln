# YoSln

* Do you want to rename a F#, C# or VB.NET project and have it move folders too?
* Do you want to update all the referencing projects and solutions regardless of whether they're in the active solution?
* Is [this solution](http://stackoverflow.com/a/224788/418492) no good for you?
* Are you comfortable on the A road to the danger zone?

If you answered yes to all of the above *and* you are drunk, this may be the project for you.

## Warning

**This is a 0.1, which means it WORKS FOR ME AND MY NEED. Your mileage will probably vary.**

This is a command line tool and is written in F#.  The work is done [here](https://github.com/bentayloruk/YoSln/blob/master/src/YoSln/Program.fs).

## Usage

### Move a project

You would do a `moveproj` like this:

`yosln.exe moveproj --proj-name src\SuckyMcSuckName\SuckyMcSuckName.csproj --new-name SuperRadName`

You would end up with:

* `src\SuperRadName\SuperRadName.csproj`.
* All projects and solutions below `.` (current directory) having their references updated.

See `yosln.exe --help` for other options.

