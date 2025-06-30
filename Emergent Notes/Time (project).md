#business 

Plan schedule management
Define activities:
	Decomposition
	Rolling wave planning: more details for near term
	Output:
		Activity list
		Activity attributes
		Milestone

Sequence activities: relationships
	PDM (Precedence Diagramming Method):
		4 dependencies (Start, Finish): FS (most common), SS, FF, SF
	Dependency determination:
		Mandatory, discretionary, external, internal
	Lead and lag: time between 2 activities
	Output:
		Schedule network diagram
		Document updates

Estimate activity resources:
	Resourse calendars: working days and shifts
	Output:
		Activity resource requirements
		RBS (Resource Breakdown Structure)
		Document updates

Estimate activity durations:
	Expert judgement
	Analogous estimating (top-down)
	Output:
		Quantitative estimates: duration, possible results
		Document updates

Develop schedule:
	CPM (Critical Path Method): longest duration path in the [[Network diagram]], should not be delayed.
	CCM (Critical Chain Method): take into account resource constraints, add buffers (float time) to protect the chain from delays.
	Resource optimization:
		Resource leveling: adjust dates based on constraints
		Resource smoothing: optimize resource with unchanged end date
		Monte Carlo simulation: quantitative risk analysis
		Schedule compression:
			Crashing: add resources to reduce duration
			Fast track: parallel overlapped activities
		Output:
			Schedule baseline: approved version
			Project schedule: planned dates (Gantt charts)
