cmake_minimum_required(VERSION 3.16)

include("Cango")

project("Cango.ByteCommunication")

set(RequiredLibraries
	"Cango::TaskDesign"
)
RequireLibraries(RequiredLibraries)

AddModulesInDirectory(
	DIRECTORY "Modules"
	NAMES
		"Core"
		"BoostImplementations"
)

AddCXXModule(
	NAME "ByteCommunication"
	NAMESPACE "Cango"
	CXX_STANDARD 20
	HEADER_DIR Headers
	SOURCE_DIR Sources
	TESTER_DIR Testers
	LINKS
		"Cango::ByteCommunication::Core"
		"Cango::ByteCommunication::BoostImplementations"
)
