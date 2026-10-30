# Approved homepage overlay

Preserves the active Clanker release while applying Olivia's reviewed homepage: full belief statement in a shallow layout, transparent photo cutouts and red annotations, compact footer with “Show us what you can do”, corner frogs with a rounded jump, and an Olivia speech bubble on the first click of Simon's profile. The second click follows the profile link; closing the dialog resets the interaction.

The CSS and lifecycle script are applied after the existing React homepage mounts. Images are separate static PNG assets. This overlay deliberately preserves the existing demo player and footer dialog code. Package with `node site/scripts/package-approved-homepage.cjs <current-release-directory> <new-output-directory>`. The packager checks the known team-removal baseline and preserves all other files. Publish only after browser verification and retain the previous release for rollback.

The separate timeline concept is outside this homepage release.
