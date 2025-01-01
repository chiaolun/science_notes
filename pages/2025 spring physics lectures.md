# Syllabus sources
	- [[Khan Academy High School Physics]]
	- [[Crash Course Physics]]
	- [[MIT OpenCourseWare - 8.01SC | Fall 2016 | Undergraduate]]
		- Pretty awful presentation, only useful for syllabus considerations
	- https://www.feynmanlectures.caltech.edu/
- # Topics
	- ## What happens during an elastic collision between two objects?
	  id:: 67735080-d6bf-4a48-ae73-00ebb8c19179
		- ((67734f35-aa88-42fb-96ea-69aeb737b833))
		- Google Sheet
		- ### Newton's Laws of Motion
		  id:: 67735051-a87f-42c8-bdc6-d8c4752c29f0
		  wikipedia: https://en.wikipedia.org/wiki/Newton%27s_laws_of_motion
			- A body remains at rest, or in motion at a constant speed in a straight line, except insofar as it is acted upon by a force.
			  logseq.order-list-type:: number
			- At any instant of time, the net force on a body is equal to the rate at which the body's momentum is changing with time.
			  logseq.order-list-type:: number
			- If two bodies exert forces on each other, these forces have the same magnitude but opposite directions.
			  logseq.order-list-type:: number
		- ### Stages of a Collision
			- Objects approach each other with some relative velocity v, each initially experiencing no net force.
			  logseq.order-list-type:: number
			- As they get closer, they begin to repel each other with a force that strictly increases as they get closer. The force is purely a function of the distance between the two objects.
			  logseq.order-list-type:: number
			- As they push on each other, their relative velocity goes down, until they are the same velocity as each other. This is the closest they will ever get to each other.
			  logseq.order-list-type:: number
			- The two objects then begin to move away from each other, and because the force is purely a function of the distance, this process is an exact reverse of the approach. the two objects will eventually gain relative velocity -v, same magnitude but exactly opposite the direction of the initial relative velocity.
			  logseq.order-list-type:: number
		- ### Conservation of Momentum
			- By the 3rd law, the decelerating force each object is experiencing is the same in magnitude but opposite in direction.
			  By the 2nd law, the acceleration experienced is inversely proportional to the mass of each object. 
			  $m_1v_1 \rightarrow m_1v_1 + F \Delta t$
			  $m_2v_2 \rightarrow m_2v_2 -  \Delta t$
			- As a result, if you take the sum of products of masses by velocities, you get
			  $m_1 v_1 + m_2 v_2 \rightarrow m_1 (v_1 + \frac{F}{m_1} \Delta t) + m_2 (v_2 - \frac{F}{m_2} \Delta t) = m_1 v_1 + m_2 v_2$
			- As long as there are no external forces, the sum of $m$ multiplied by $v$ is always the same! This fact is called the conservation of momentum, and it follows directly from Newton's Laws.
		- ### Center of Mass
			- Using the conservation of momentum, we can find the velocity that the two objects reach in stage 3, at the moment of closest approach. We call that velocity $v_c$. It's the center-of-mass velocity
			  $m_1v_1 + m_2v_2 = (m_1 + m_2)v_c$
			- We express initial velocities $v_1$ and $v_2$ relative to $v_c$
			  $v_{i1} = v_c + u_1$
			  $v_{i2} = v_c + u_2$
			- The final velocities are thus
			  $v_{f1} = v_c - u_1$
			  $v_{f2} = v_c - u_2$
		- ### Kinetic energy
			- Define kinetic energy as $\frac{1}{2} m_iv_i^2$
			- Total initial kinetic energy:
			  $\frac{1}{2}m_1v_{i1}^2 + \frac{1}{2}m_2v_{i2}^2 = \frac{1}{2}m_1(v_c + u_1)^2 + \frac{1}{2}m_2(v_c + u_2)^2$
			- Total final kinetic energy:
			  $\frac{1}{2}m_1v_{f1}^2 + \frac{1}{2}m_2v_{f2}^2 = \frac{1}{2}m_1(v_c - u_1)^2 + \frac{1}{2}m_2(v_c - u_2)^2$
			- Change in total kinetic energy:
			  $-2v_c(m_1 u_1 + m_2 u_2)$
			- Equation for $v_c$:
			  $m_1v_1 + m_2v_2 = (m_1 + m_2)v_c$
			  $m_1(v_1 - v_c) + m_2(v_2 - v_c) = 0$
			  $m_1u_1 + m_2u_2 = 0$
			- Therefore, the change in kinetic energy is zero
		- ### Questions
			- Is total momentum the same throughout the interaction?
				- Yes! It follows from the 2nd and 3rd laws, and always holds.
			- Is total kinetic energy the same throughout the interaction?
				- No! We only showed it was the same before and after the collision. During the collision kinetic energy goes down and is minimal at the point of closest approach. Consider the case where two objects come in from the left and the right and are stationary at the point of closest approach - the kinetic energy is zero at that time!
			- What is the assumption that we've made that tells us the total kinetic energy before and after the collision will be the same?
				- The only assumption we have made is that the force with which objects push each other depends only on the distance between them.
				- Over the course of a collision, they are at any particular inter-object distance exactly twice - the first time while decelerating and the second time while accelerating, with respect to a special velocity $v_c$.
		- ### Special cases
		  | Case | $m_1$ | $m_2$ | $v_{1i}$ | $v_{2i}$ | $v_c$ | $u_1$ | $u_2$ | $v_{1f}$ | $v_{2f}$ |
		  |------|-------|-------|-----------|-----------|--------|--------|--------|-----------|-----------|
		  | Equal masses | $m$ | $m$ | $v$ | $0$ | $v/2$ | $v/2$ | $-v/2$ | $0$ | $v$ |
		  | Massive $m_2$ | $m$ | $\infty$ | $v$ | $0$ | $0$ | $v$ | $0$ | $-v$ | $0$ |
		  | Massive $m_1$ | $\infty$ | $m$ | $v$ | $0$ | $v$ | $0$ | $-v$ | $v$ | $2v$ |
		- ### Related phenomena
			- Gravity assist - https://youtube.com/shorts/kD8PFhj_a8s - nothing in our analysis says the force needs to be a push, a pull can work as well. Gravity assists slow down planets a bit in exchange for speeding up the spacecraft a lot. Which special case is it? What does this tell us about the maximum speed boost you get?
- # Classes
	- [[2025-02-20 physics]]
	  logseq.order-list-type:: number
	- [[2025-03-06 physics]]
	  logseq.order-list-type:: number
	- [[2025-03-13 physics]]
	  logseq.order-list-type:: number
	- [[2025-03-20 physics]]
	  logseq.order-list-type:: number
	- [[2025-03-27 physics]]
	  logseq.order-list-type:: number
	- [[2025-04-10 physics]]
	  logseq.order-list-type:: number
	- [[2025-04-17 physics]]
	  logseq.order-list-type:: number
	- [[2025-04-24 physics]]
	  logseq.order-list-type:: number
	- [[2025-05-01 physics]]
	  logseq.order-list-type:: number
	- [[2025-05-08 physics]]
	  logseq.order-list-type:: number
	- [[2025-05-15 physics]]
	  logseq.order-list-type:: number
	- [[2025-05-22 physics]]
	  logseq.order-list-type:: number
	- [[2025-05-29 physics]]
	  logseq.order-list-type:: number
	- [[2025-06-05 physics]]
	  logseq.order-list-type:: number
	- [[2025-06-12 physics]]
	  logseq.order-list-type:: number
	- [[2025-06-19 physics]]
	  logseq.order-list-type:: number
	- [[2025-06-26 physics]]
	  logseq.order-list-type:: number