# Release process

1. `npm upgrade`
2. `npm run i18n:fields`
3. Check for differences in `src/locales/en/fields.json`
4. Ask for missing translations via GitHub issues
5. Update the version number (in `package.json` and `README.md`)
6. `npm run lint` - Fix any open lint issues
7. Commit the changes
8. `npm run build:report`
9. Check whether the `dist/report.html` has significantly changed (if yes, check why)
10. Delete the `dist/report.html`
11. `npm publish`
12. Create GitHub release (v3.x.x)
