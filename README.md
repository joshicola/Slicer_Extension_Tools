# Slicer Extension Tools

This is a repository to support the Flywheel 3D Slicer Extensions and their use.

## The 3D Slicer Extensions

The Flywheel 3D Slicer Extensions are a set of tools that allow users to interact with
Flywheel data directly from 3D Slicer. The extensions are designed to be used in
conjunction with a Flywheel Instance via an API. The extensions provide a way
to visualize and analyze Flywheel data in 3D Slicer, and to upload the results back to
Flywheel.

Both of these extensions are available in the 3D Slicer Extension Manager.

### Flywheel Connect

The [Flywheel
Connect](https://gitlab.com/flywheel-io/scientific-solutions/app/slicer_flywheel_connect)
extension allows users to connect to a Flywheel instance and browse through the data in
a hierarchical manner. The extension provides a way to download data from Flywheel to
the local machine, manipulate that data in 3D Slicer, and to upload the results back to
Flywheel.

### Flywheel Case Iterator

The [Flywheel Case
Iterator](https://gitlab.com/flywheel-io/scientific-solutions/app/Slicerflywheelcaseiterator)
extension allows users to iterate through a set of cases in Flywheel. This allows the
user to segment and analyze a set of cases in a batch manner without navigating through
a hierarchy tree.

## Extension Tools

### Prepare Cases

The Flywheel Case Iterator depends on producing a list of cases to iterate through (CSV
file). The `Prepare Cases` tool allows the user to specify a Flywheel project and a set
of criteria to filter the cases. The tool will then produce a list of cases that can be
iterated through. Furthermore, the tool will ensure that additional images and masks are
associated with each case according to the user's specifications.

For now, the `Prepare Cases` tool is only available as a [Jupyter
Notebook](prepare_cases.ipynb).
