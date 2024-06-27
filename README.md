

This present work aimed to enhance ore exports and reduce demurrage fines and costs at the port's mining company using multicriteria decision-making models and methods. The global mining supply chain encompasses multiple stages, with port production logistics being a crucial aspect. This stage involves planning the production volume allocated to vessels for transporting ore to its final destination. However, uncertainties arise during this process, including the volume produced and associated operational costs and fines. Traditionally, deterministic monocriteria models have been employed for decision-making, aiming to optimize outcomes without considering uncertainty factors. Nevertheless, given the nature of the problem, the solution should be implemented within a multicriteria decision-making framework under conditions of uncertainty. The analysis is based on applying the General Multicriteria Decision-Making using <X, F> and <X, R> models to solve multicriteria problems and provide their harmonious solutions. The objective is to assist decision-makers in planning ore production shipped from mining company ports, utilizing a multicriteria system instead of a monocriteria. A case study was conducted at a Brazilian mining company exporting iron ore in their ports, comparing the current monocriteria approach with the multicriteria. The simulated results were compared with the real ports operations. The study concludes that utilizing the <X, F> and <X, R> models, the general multicriteria decision-making approach demonstrated effectiveness in allocating ore production at mining company ports, providing analytical and practical advantages.



Key words-mining supply chain; port logistics; multicriteria decision-making; uncertainty.


# INTRODUCTION 

Ores are basic raw materials in numerous sectors of the global economy [1]. They are primarily transported through maritime shipping and constitute over 80% of international trade [2]. In Brazil, the export of raw iron ore accounts for more than 29% of the country's total port exports [3].
Considering their significant economic and social importance, the management and control of all ores involve a complex supply chain with inherent uncertainties throughout the operation. Port operations are crucial in the production flow, from its movement to the final delivery to end customers. These operations coordinate the dispatch and receipt of resources via maritime transportation. Consequently, the intricate nature of port operations arises from the high volume of product circulation and the pressure to meet the deadlines of all involved parties [4].
While addressing the challenges of production flow and ship planning at ports, the available literature directly connected to mining is limited, as highlighted by [5]. Furthermore, most existing solutions for these problems rely on deterministic and single-criteria models, disregarding uncertainty factors [5].
However, the complexities of these problems involve multiple decisions and objectives, such as maximizing production volume and minimizing associated costs. Thus, these problems inherently entail a multicriteria nature, where decision-making is based on conflicting criteria [6].
Hence, approaches considering the underlying uncertainties in the production flow and maritime transportation would significantly contribute to the existing literature. Particularly, the capability of quantifying uncertainty and optimizing systems under mapped uncertainties would be valuable advancements in the field [5][7].
Consequently, the results obtained by [8] provide a general framework for analyzing multi-objective problems (analysis of <X, F>). And if it's necessary to distinguish the solutions after the decision-making analysis, it's possible to use <X, R> models to try to find the more robust final solution. So, this framework incorporates the uncertainty factor within a possibilistic approach to generate robust (non-dominated) solutions, as emphasized by [9] and [10].
In light of these considerations, utilizing a general framework for analyzing multicriteria problems offers a robust solution for the flow of ore production through resource allocation. This article contributes methodologically and practically to both mining companies and academic research by employing a general framework for analysis.
THE PORT PROCESS

Port terminals serve as a link between ore production and delivery. Therefore, ports must not act as bottlenecks in the operation. They should ensure a continuous flow in the railways by storing the received ores in their limited storage yard, thus avoiding delays in ships and penalties, such as demurrage [5].
As mentioned, there is a need to plan how and when ships will be allocated to transport ore production to its final destination. This advanced planning usually takes place in two-time windows: medium-term (next 6 months) and short-term (next 3 months). The scope of this study will focus on medium-term planning. In this planning process, the decision-maker analyzes the projected input data. The main data include Production volume; Port capacity to support vessel loading operations; Customer demand; and available ships for the operation.
With this data, the planner requests a forecast from the current ship allocation software (monocriteria and deterministic function) to determine which vessels should be chosen. Once the vessels are identified, the decision-maker charters the ships for the upcoming months. It is important to note that this process is carried out for all ports of the mining company.
However, this process is more complex than it appears, as there are many uncertainties involved in this decision. This is because if the production flow exceeds the contracted capacity, the mining company will need to go to the market and charter additional vessels at a higher price than planned (spot chartering). If the previously contracted ships are insufficient, there is also the risk of the mining company not finding available vessels, resulting in delays in delivery and increased port costs.
On the other hand, the mining company may charter more ships than necessary due to optimistic planning. This can result in delays in vessel loading due to the high volume of ships. The delay in ore shipment to the vessels leads to increased port costs due to extended berthing time. Additionally, demurrage charges increase as the vessels stay in ports longer than anticipated.
Ideally, the planning should be as realistic as possible to minimize port costs and efficiently dispatch production. With a more accurate planning approach, it would be possible to minimize both the cost of spot chartering and demurrage charges.
Thus, there is an opportunity to conceive and implement approaches based on mathematical models to deal with these uncertainties and their constraints. The objective is to create a more efficient plan that minimizes operational and demurrage costs while optimally utilizing reserve capacity to maximize productivity.

#RELATED WORKS
The problem of ship allocation in ports has been addressed in several research studies aiming to minimize port operational costs. Various objectives have been considered, such as reducing ship idle time and minimizing penalties for delays [5][11]-[14]. These approaches have ranged from applying single-criterion models to utilizing stochastic techniques and fuzzy sets [15]-[19]. However, the majority of these works did not consider the maximization of cargo throughput and the minimization of port costs and demurrage penalties as primary objectives. Additionally, they did not explore the multicriteria decision-making approach using the <X, F> and <X, R> models. Therefore, this research stands out by considering uncertainty factors in the ore production process and port costs, applying multicriteria models to assist the planner's decision-making process. The objective is to contribute to the advancement of research related to ore production flow in mining ports.

#METHODOLOGY

The current modeling approach adopted by the mining company is a monocriteria objective function.
In essence, the program, based on the input data, aims to find an optimal value by simultaneously reducing costs and ensuring the fulfillment of predicted demands through tracking routes and available vessels.
Additionally, fixed coefficients are associated with each of the objective functions to scale and weigh them. The rationale behind using these coefficients is that they expedite the optimization process by guiding the model toward the desired outcome.
The approach adopted by the mining company aligns with the monocriteria convolution process, where a scaling process of the objective functions occurs. However, these functions are not normalized, as they undergo a resizing process.
Moreover, the fixed coefficients serve a different purpose than the uncertainty factors mentioned by [6] and [8], which are used to prioritize equations in the convolution process.
While this fixed fine-tuning process can be advantageous in certain scenarios, it may result in unsatisfactory solutions if unforeseen circumstances arise. This issue has been observed in the literature [5].
Based on expert's opinions, literature reviews, and related works, the following objectives have been established:
Predominantly making the produced ore available for the mining company's ports (Amount).
Predominantly limiting the costs associated with keeping vessels docked while being loaded at the mining company's port piers (PortExp).
Predominantly limiting the fuel consumption of vessels transporting the ore to final customers from the mining company's ports (Bunker).
Predominantly limiting demurrage at each of the mining company's ports (Demu).
Predominantly limiting the daily cost of chartering a vessel (Time Charter) at each of the mining company's ports (TC).
Additionally, the model incorporates the following constraints:
Restriction on the storage capacity of the ore produced at the mining company's ports.
The estimated cost of keeping docked (PortExp) is limited by the number of vessels, time period, and origin and destination ports.
The cost of vessel fuel consumption (Bunker) is restricted by the type of fuel used on a specific date for a set of planned vessels and ports.
Demurrage (Demu) is constrained by the planned value for the respective year.
The daily cost of chartering a vessel (TC) is limited by the number of vessels used at the mining company's ports and the destination ports for a given month.
The uncertainties in the objective functions are defined through uncertainty intervals. These minimum and maximum intervals are generated by analyzing the mining company's historical data.
The minimum and maximum values are obtained by averaging the specific costs for the month and port under analysis.
Consequently, it is possible to construct the objective functions with their respective applied uncertainties (1), (2), (3), and (4).

#CASE STUDY
For the case study, an estimate of production flow at the ports for July 2021 was simulated, along with the associated costs and demurrage penalties for the same period.
Comparing the actual results obtained by the mining company with the simulated results from the monocriteria and multicriteria approaches, we can derive the following findings.
Starting with the "Amount" objective, the following percentage values relative to the actual value can be observed, as shown in Table 1:
Ports
Monocriteria
Multicriteria
Port 1
213,65%
97,28%
Port 2
55,96%
63,25%
Port 3
695,53%
253,67%
Port 4
31,29%
157,96%
Total
322,88%
161,72%

Table 1: Comparison of the production result predicted by the monocriteria and multicriteria approach with the actual one.
It is possible to verify from Table 1 that the simulation values are either overly optimistic or pessimistic when compared to reality, which greatly hinders the accuracy of the mining company's tactical planning. As observed, the multicriteria solution founded is more harmonious and robust when compared to the actual results for the same period. In some cases, such as Port 1, the difference is as low as 2.72%. This is due to the fact that the general decision-making scheme utilizes the <X, F> and <X, R> models, enabling the identification of the scenario with the highest degree of non dominance possible.
Now, comparing the actual results of costs and demurrage penalties, we arrive at the corresponding values depicted in Figures 1.
Figure 1 - Comparative graphs of costs minimized by monocriteria and multicriteria approaches
It can be observed that most of the costs predicted by the multicriteria approach were lower when compared to the predictions obtained from the monocriteria analysis.
With cost forecasts, the freight that can be charged, and the volume of production, the decision-maker will be able to make more accurate decisions regarding the number of ships to be used to facilitate delivery to customers. This will help reduce operational costs as well as demurrage penalties, thereby increasing the net profit margin.

#CONCLUSIONS

As seen, the global mining supply chain is complex, with multiple stages and uncertainties associated with each of them. Among these areas, this study focused on addressing the problem of production flow at the ports of a mining company. In this problem, based on the literature review, the main variables of uncertainty were identified in relation to maximizing the volume of flow and minimizing port operation costs and penalties.
Furthermore, it was identified in the problem that the current mining company has an "optimistic" and deterministic approach to ore production, which directly affects costs and the uncertainty of the information provided to the model. Therefore, a multicriteria objective function modeling approach was proposed to assist decision-makers in selecting the most harmonious solution.
Based on the final results, it can be concluded that the multicriteria decision-making approach using the <X, F> and <X, R> models proved to be effective for allocating ore production at the company's ports. In this sense, two conclusions can be drawn from our work.
The first one is an analytical advantage. Although the mining company does not use the proposed modeling in its actual operations, this work demonstrates that this problem, under a deterministic approach, has intervals or factors of uncertainty that were not initially considered. Thus, we have a theoretically insufficient model for informed uncertainty, and a monocriteria application is not the best strategy for making decisions.
The second is a practical advantage, as the work presents a way to solve the proposed problem through multicriteria models <X, F> and <X, R>, making the decision-making process pragmatic, with robust and harmonious solutions. This generates a more realistic plan aiming to reduce port costs and increase production flow for the vessels.

REFERENCES:
[1] SEONG, J. et al. November 2022 global flows: The ties that bind in an interconnected world. McKinsey Global Institute, McKinsey, 2022.
[2] HOFFMANN, J. et al. UNCTAD: Review of maritime transport 2022. [S.l.]: United Nations Publications, 2022. 
[3] ANTAQ. Estatístico Aquaviário 2022. ANTAQ - Agência Nacional de Transportes Aquaviários, 2022.
[4] WENDLER-BOSCO, V.; NICHOLSON, C. Port disruption impact on the maritime supply chain: a literature review. Sustainable and Resilient Infrastructure, Taylor & Francis, v. 5, n. 6, p. 378–394, 2020.
[5] LEITE, J. G. et al. Modeling the integrated mine-to-client supply chain: a survey. Int. J. Min. Reclamat. Environ., v. 1579693, 2019.
[6] ZHANG, G. quan et al. Multi-objective Group Decision Making: Methods Software And Applications With Fuzzy Set Techniques (With Cd-rom). World Scientific Publishing Company, 2007. (Series In Electrical And Computer Engineering).
[7] YU, J. et al. Ship arrival prediction and its value on daily container terminal operation. Ocean Engineering, Elsevier, v. 157, p. 73–86, 2018.
[8] EKEL, P.; PEDRYCZ, W.; Pereira Jr., J. Multicriteria decision-making under conditions of uncertainty: A fuzzy set perspective. [S.l.]: John Wiley & Sons, 2020.
[9] Pereira Jr, J. et al. On multicriteria decision making under conditions of uncertainty. Information Sciences, v. 324, p. 44–59, 2015.
[10] EKEL, P. et al. Multiobjective and multiattribute decision making in a fuzzy environment and their power engineering applications. Information Sciences, v. 361-362, p. 100–119, 2016.
[11] WANG, W. et al. Integrated scheduling of port-centric supply chain: A special focus on the seaborne uncertainties. Journal of Cleaner Production, Elsevier, v. 262, p. 121240, 2020.
[12] SHIH, L.-H. Planning of fuel coal imports using a mixed integer programming method. International journal of production economics, Elsevier, v. 51, n. 3, p. 243–249, 1997
[13] BOLAND, N. et al. Improved stockyard management strategies for coal export terminals at newcastle. In: Proceedings of the 19th International Congress on Modelling and Simulation. [S.l.: s.n.], 2011. p. 718–724.
[14] BOLAND, N.; GULCZYNSKI, D.; SAVELSBERGH, M. A stockyard planning problem. EURO Journal on Transportation and Logistics, Elsevier, v. 1, n. 3, p. 197–236, 2012.
[15] EXPÓSITO-IZQUIERO, C. et al. Fuzzy optimization models for seaside port logistics: Berthing and quay crane scheduling. In: . Computational Intelligence: Revised and Selected Papers of the International Joint Conference, IJCCI 2013, Vilamoura, Portugal, September 20-22, 2013. Cham: Springer International Publishing, 2016. p. 323–343. 
[16] SEGURA, F. G. et al. A fully fuzzy linear programming model to the berth allocation problem. In: IEEE. 2017 Federated Conference on Computer Science and Information Systems (FedCSIS). [S.l.], 2017. p. 453–458.
[17] GUTIERREZ, F. et al. Fully fuzzy linear programming model for the berth allocation problem with two quays. In: . Uncertainty Management with Fuzzy and Rough Sets: Recent Advances and Applications. Cham: Springer International Publishing, 2019. p. 87–113.
[18] GUTIERREZ, F. et al. Fuzziness in the berth allocation problem. In: . Recent Advances in Computational Optimization: Results of the Workshop on Computational Optimization WCO 2017. Cham: Springer International Publishing, 2019. p. 149–174.
[19] PÉREZ-CAÑEDO, B. et al. Fully fuzzy multi-objective berth allocation problem. In: CAL, E. A. de la et al. (Ed.). Hybrid Artificial Intelligent Systems. Cham: Springer International Publishing, 2020. p. 261–272.
