@startuml
!define ArrowColor #333333
!define FontColor #333333
!define BoxColor #FFFFFF
!define LineColor #CCCCCC

skinparam backgroundColor #FFFFFF
skinparam rectangle {
    BackgroundColor BoxColor
    BorderColor LineColor
    FontColor FontColor
}
skinparam node {
    FontColor FontColor
}
skinparam arrow {
    Color ArrowColor
}

entity "抖音平台娱乐性" as DY_Entertainment {
    *丰富娱乐内容（搞笑视频、才艺表演等）
    *创新互动玩法（话题挑战、合拍功能等）
}

entity "年轻用户社交偏好" as YU_SocialPreference {
    *积极分享品牌信息
    *参与话题讨论与互动
    *构建社交圈子
}

entity "品牌年轻化转型" as Brand_Rejuvenation {
    *产品创新
    *品牌形象重塑
    *营销渠道拓展
    *传播内容创新
}

entity "年轻用户社交活跃度" as YU_ActivityLevel {
    *点赞、评论、分享频率
    *参与话题讨论和挑战活动积极性
}

entity "品牌与年轻用户互动频率" as Brand_Interaction {
    *回复用户评论
    *举办线上活动邀请用户
    *开展用户调研
}

DY_Entertainment --> Brand_Rejuvenation : 直接影响 (H3)
DY_Entertainment --> YU_SocialPreference : 正向影响 (H1)
YU_SocialPreference --> Brand_Rejuvenation : 正向影响 (H2)

YU_ActivityLevel --> (DY_Entertainment --> Brand_Rejuvenation) : 调节作用 (H4)
Brand_Interaction --> (YU_SocialPreference --> Brand_Rejuvenation) : 调节作用 (H5)

@enduml

