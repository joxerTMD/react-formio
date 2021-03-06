# Change Log 
All notable changes to this project will be documented in this file

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]

## 1.3.12
### Added
 - Events that fire when select lists open or close.
 - Event that fires on add/remove from datagrid.
 - Event that fires on loadMore for selects.

## 1.3.11
### Reverted
 - Reverted revert of change to datagrids delete value.
 
### Fixed
 - Calculated Select values could return something other than an array which caused an error.

## 1.3.10
### Reverted
 - Reverted change to setting values that attempted to fix deleting rows in datagrids issue that had a lot of side effects.

### 1.3.9
### Fixed
 - Fix MinLength calculation for datagrids.
 - Fixed error about setState in select component.
 - Scenario where updating a form doesn't always set the values.
 
### Changed
 - Replace full lodash with individual functions.

## 1.3.8
### Fixed
 - Datagrids with select components dependent on external data weren't updating when the data updated.

## 1.3.7
### Changed
 - Datagrid headers won't render if there are no labels.

## 1.3.6
### Fixed
 - Deleting rows in datagrids didn't clear components properly.

## 1.3.5
### Fixed
 - Fix performance of datagrids with large data.

## 1.3.4
### Added
 - Onchange event will fire for input fields after 500ms of no typing instead of only on blur.

## 1.3.3
### Added
 - Expose mixins as exports to ease creation of custom components.

## 1.3.2
Changed
 - Text inputs will fire change events on blur now instead of on change. Change events were too slow in redux.

## 1.3.1
### Fixed
 - Fixed tests dealing with input mask change and missing onChange events. 

### Removed
 - Removing tests that don't work with current libraries.

## 1.3.0
### Changed
 - Swapped react-input-mask for react-text-mask for input masks.
 - Improved performance of input masks.
