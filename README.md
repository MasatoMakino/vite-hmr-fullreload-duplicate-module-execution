# vite-hmr-fullreload-duplicate-module-execution
A minimal reproduction of an issue in Vite where module top-level code is executed multiple times when using both HMR and Full Reload together.

This repository demonstrates how global scope code (outside of functions) runs repeatedly during development when TypeScript files are modified, requiring manual initialization guards. The issue does not occur when using HMR alone without Full Reload.
